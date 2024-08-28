# CDC
postgres + debezium + kafka

https://www.youtube.com/watch?v=YZRHqRznO-o

### POSTGRES

```sql
CREATE TABLE student (id integer primary key, name varchar );

SELECT * FROM student;

ALTER TABLE public.student REPLICA IDENTITY FULL;
```


### DEBEZIUM

Setup
```shell
curl -i -X POST -H "Accept:application/json" -H "Content-Type:application/json" 127.0.0.1:8083/connectors/ --data "@debezium.json"
```

### KAFKA
