# Choosing Fargate task sizes<a name="fargate-task-size"></a>

If you run your tasks on AWS Fargate, you must declare the task CPU and memory limits in your task definition\. ECS uses these limits to determine the Fargate instance type to run your task on\. The limits that you determine must be greater than or equal to any reservations that you declared\. In most cases, you can set them to the sum of the reservations of each of the container that's declared in your task definition\. Then, also round the number up to the nearest Fargate instance size\. For more information about the available sizes, see [Task CPU and memory](AmazonECS/latest/developerguide/AWS_Fargate.html#fargate-tasks-size) in the *Amazon Elastic Container Service Developer Guide*\. 