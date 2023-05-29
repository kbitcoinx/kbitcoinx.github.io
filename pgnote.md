### The Note of PostgreSQL DBA Job

recovery.conf
```
restore_command='/usr/bin/true'
recovery_target = 'immediate'

```

### Common SQLs
```sql

select current_timestamp - pg_postmaster_start_time() as uptime;
select pg_postmaster_start_time() as uptime;
SELECT * FROM pg_stat_replication;
select * from pg_replication_slots;
SELECT pg_is_in_recovery();
SELECT * FROM pg_tablespace;
SELECT pg_size_pretty(pg_database_size('datanamename')); 


```

### Common OS Commands
```
cat /etc/postgresql/9.6/main/postgresql.conf | grep -v ^$ | grep -v ^[[:space:]]*\#
-- list all service of systemctl
sudo systemctl --type=service | grep postgres

```
