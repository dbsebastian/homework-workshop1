## homework-workshop1

### Q1

'''
def square_root_generator(limit):  
    n = 1
    while n <= limit:
        yield n ** 0.5
        n += 1

limit = 5
generator = square_root_generator(limit)

sumat = 0
for sqrt_value in generator:
    sumat += sqrt_value
    print(sqrt_value)

print("")
print(f"la sumatoria es: {sumat}")
'''

[8.382]



### Q2

[3.605]




### Q3

'''
SELECT SUM ( age) 
FROM users;
'''

[353]


### Q4

'''
data = list()

for person in people_1():
    data.append(person)
    print(person)

print(data)


pipeline = dlt.pipeline(pipeline_name="pipe_personas",
                        destination='duckdb', 
                        dataset_name='personas'
                        )

info = pipeline.run(data, 
                    table_name="users", 
                    write_disposition="append"
                    )


print(info)

print("----------------------------")

data = list()

for person in people_2():
    data.append(person)
    print(person)

print(data)

pipeline = dlt.pipeline(pipeline_name="pipe_personas",
                        destination='duckdb', 
                        dataset_name='personas'
                        )

info = pipeline.run(data, 
                    table_name="users", 
                    write_disposition="merge",
                    primary_key='ID'
                    )


print(info)
'''

'''
SELECT SUM ( age) 
FROM users;
'''

[266]
