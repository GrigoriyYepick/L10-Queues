# L10-Queues
 

## Build:
Pick one of approaches (beanstalkd, redis_aof, redis_rdb) and build docker-compose in that folder.

```
docker-compose build

docker-compose up -d
```

## Results:


### Beanstalkd
![Results](https://github.com/GrigoriyYepick/L10-Queues/blob/main/beanstalkd/siege.txt)

```
+-------------+--------+------------------------+
| Concurrency |  Time  | Trasactions per second |
+-------------+--------+------------------------+
|   10        |  30s   |     502                |
+-------------+--------+------------------------+
|   25        |  30s   |     233                |
+-------------+--------+------------------------+
|   50        |  30s   |     10                 |
+-------------+--------+------------------------+
```

### Redis AOF
![Results](https://github.com/GrigoriyYepick/L10-Queues/blob/main/redis_aof/siege.txt)

```
+-------------+--------+------------------------+
| Concurrency |  Time  | Trasactions per second |
+-------------+--------+------------------------+
|   10        |  30s   |     455                |
+-------------+--------+------------------------+
|   25        |  30s   |     160                |
+-------------+--------+------------------------+
|   50        |  30s   |     9                  |
+-------------+--------+------------------------+
```

### Redis RDB
![Results](https://github.com/GrigoriyYepick/L10-Queues/blob/main/redis_rdb/siege.txt)

```
+-------------+--------+------------------------+
| Concurrency |  Time  | Trasactions per second |
+-------------+--------+------------------------+
|   10        |  30s   |     450                |
+-------------+--------+------------------------+
|   25        |  30s   |     213                |
+-------------+--------+------------------------+
|   50        |  30s   |     24                 |
+-------------+--------+------------------------+
```
