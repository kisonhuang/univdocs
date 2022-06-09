# Runner

```java
org.springframework.boot.ApplicationRunner
    + org.springframework.boot.autoconfigure.batch.JobLauncherApplicationRunner
        + org.springframework.boot.autoconfigure.batch.JobLauncherCommandLineRunner

org.springframework.boot.CommandLineRunner
org.springframework.boot.loader.MainMethodRunner
```

## ApplicationRunner

```java
org.springframework.boot.ApplicationRunner
+ run(ApplicationArguments)
```

## JobLauncherApplicationRunner

```java
org.springframework.boot.autoconfigure.batch.JobLauncherApplicationRunner
+ DEFAULT_ORDER
+ JobLauncherApplicationRunner(JobLauncher, JobExplorer, JobRepository)
+ run(String...)
+ run(ApplicationArguments)
+ getOrder()
+ setApplicationEventPublisher(ApplicationEventPublisher)
+ setJobNames(String)
+ setJobParametersConverter(JobParametersConverter)
+ setJobRegistry(JobRegistry)
+ setJobs(Collection<Job>)
+ setOrder(int)
```

## JobLauncherCommandLineRunner废弃

```java
org.springframework.boot.autoconfigure.batch.JobLauncherCommandLineRunner
+ JobLauncherCommandLineRunner(JobLauncher, JobExplorer, JobRepository)
```

## CommandLineRunner

```java
org.springframework.boot.CommandLineRunner
+ run(String...)
```

## MainMethodRunner

```java
org.springframework.boot.loader.MainMethodRunner
+ MainMethodRunner(String, String[])
+ run()
```




