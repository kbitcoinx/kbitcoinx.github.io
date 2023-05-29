### The Note of PostgreSQL DBA Job

recovery.conf
```
restore_command='/usr/bin/true'
recovery_target = 'immediate'

```

### Common SQLs
```sql
select pg_is_in_recovery();
```
