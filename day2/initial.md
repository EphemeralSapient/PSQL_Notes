I haven't delved deep into WAL records and stuff previously so I've decided to follow up on that today;

Even through none of these topics are organized in proper order, I believe It at least tracks my progress [maybe i'll organize it someday as per concept]

Let's explore log generated by PostgreSQL today and make sure to configure your PostgreSQL's config file

For myself, in linux, it is found on `/var/lib/postgres/data/postgresql.conf` 

I've modified to enable 

```
log_parser_stats = on
log_planner_stats = on
log_executor_stats = on
```

	log format to be jsonlog instead of stderr 

and other relevent config to be enabled as per your findings :P 

Once done, make sure to restart the postgresql [ `sudo systemctl restart postgresql.service` ]

We will be using **jless** for viewing JSON file so, download if you need or use preferred text editor like VSCode 

> Moving onto [log.md](./log.md)


