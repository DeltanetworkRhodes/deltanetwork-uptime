# deltanetwork-uptime

Ωριαίος/δεκάλεπτος έλεγχος ότι η παραγωγή του DeltaNetwork.app ζει, με ειδοποίηση στο κινητό μέσω ntfy.

- Supabase `/auth/v1/health` → 401 (ζει) · 540 (paused)
- `deltanetwork.app` → 200

Public repo επίτηδες: τα Actions των public repos είναι δωρεάν. Το ntfy topic ζει σε repository secret (`NTFY_TOPIC`), ποτέ στον κώδικα.

Τα scheduled workflows απενεργοποιούνται αν το repo μείνει 60 μέρες χωρίς commit — το GitHub στέλνει email πριν.
