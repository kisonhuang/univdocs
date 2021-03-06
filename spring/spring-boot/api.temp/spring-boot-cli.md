# CLI 93

```java
org.springframework.boot.cli.command.CommandRunner
org.springframework.boot.cli.command.run.SpringApplicationRunner

org.springframework.boot.cli.compiler.GroovyCompilerConfiguration
    + org.springframework.boot.cli.command.run.SpringApplicationRunnerConfiguration
    + org.springframework.boot.cli.command.options.OptionSetGroovyCompilerConfiguration
```




# Spring Boot API

## 枚举

org.springframework.boot.cli.command.CommandException.Option
org.springframework.boot.cli.compiler.GroovyCompilerScope

## 接口

org.springframework.boot.cli.command.Command
org.springframework.boot.cli.command.CommandFactory
org.springframework.boot.cli.command.options.OptionHelp
org.springframework.boot.cli.compiler.SpringBootAstTransformation
org.springframework.boot.cli.compiler.dependencies.ArtifactCoordinatesResolver
org.springframework.boot.cli.compiler.dependencies.DependencyManagement
org.springframework.boot.cli.compiler.grape.RepositorySystemSessionAutoConfiguration

## 类

org.springframework.boot.cli.DefaultCommandFactory
org.springframework.boot.cli.SpringCli
org.springframework.boot.cli.app.SpringApplicationLauncher
org.springframework.boot.cli.app.SpringApplicationWebApplicationInitializer
org.springframework.boot.cli.archive.PackagedSpringApplicationLauncher
org.springframework.boot.cli.command.AbstractCommand
org.springframework.boot.cli.command.HelpExample
org.springframework.boot.cli.command.OptionParsingCommand
org.springframework.boot.cli.command.archive.JarCommand
org.springframework.boot.cli.command.archive.WarCommand
org.springframework.boot.cli.command.core.HelpCommand
org.springframework.boot.cli.command.core.HintCommand
org.springframework.boot.cli.command.core.VersionCommand
org.springframework.boot.cli.command.encodepassword.EncodePasswordCommand
org.springframework.boot.cli.command.grab.GrabCommand
org.springframework.boot.cli.command.init.InitCommand
org.springframework.boot.cli.command.install.InstallCommand
org.springframework.boot.cli.command.install.UninstallCommand
org.springframework.boot.cli.command.options.CompilerOptionHandler
org.springframework.boot.cli.command.options.OptionHandler
org.springframework.boot.cli.command.options.SourceOptions
org.springframework.boot.cli.command.run.RunCommand
org.springframework.boot.cli.command.shell.CommandCompleter
org.springframework.boot.cli.command.shell.PromptCommand
org.springframework.boot.cli.command.shell.Shell
org.springframework.boot.cli.command.shell.ShellCommand
org.springframework.boot.cli.command.shell.ShellPrompts
org.springframework.boot.cli.command.status.ExitStatus
org.springframework.boot.cli.compiler.AnnotatedNodeASTTransformation
org.springframework.boot.cli.compiler.AstUtils
org.springframework.boot.cli.compiler.CompilerAutoConfiguration
org.springframework.boot.cli.compiler.DependencyAutoConfigurationTransformation
org.springframework.boot.cli.compiler.DependencyCustomizer
org.springframework.boot.cli.compiler.DependencyManagementBomTransformation
org.springframework.boot.cli.compiler.ExtendedGroovyClassLoader
org.springframework.boot.cli.compiler.GenericBomAstTransformation
org.springframework.boot.cli.compiler.GroovyBeansTransformation
org.springframework.boot.cli.compiler.GroovyCompiler
org.springframework.boot.cli.compiler.RepositoryConfigurationFactory
org.springframework.boot.cli.compiler.ResolveDependencyCoordinatesTransformation
org.springframework.boot.cli.compiler.autoconfigure.CachingCompilerAutoConfiguration
org.springframework.boot.cli.compiler.autoconfigure.GroovyTemplatesCompilerAutoConfiguration
org.springframework.boot.cli.compiler.autoconfigure.JdbcCompilerAutoConfiguration
org.springframework.boot.cli.compiler.autoconfigure.JmsCompilerAutoConfiguration
org.springframework.boot.cli.compiler.autoconfigure.RabbitCompilerAutoConfiguration
org.springframework.boot.cli.compiler.autoconfigure.SpringBatchCompilerAutoConfiguration
org.springframework.boot.cli.compiler.autoconfigure.SpringBootCompilerAutoConfiguration
org.springframework.boot.cli.compiler.autoconfigure.SpringIntegrationCompilerAutoConfiguration
org.springframework.boot.cli.compiler.autoconfigure.SpringMvcCompilerAutoConfiguration
org.springframework.boot.cli.compiler.autoconfigure.SpringRetryCompilerAutoConfiguration
org.springframework.boot.cli.compiler.autoconfigure.SpringSecurityCompilerAutoConfiguration
org.springframework.boot.cli.compiler.autoconfigure.SpringTestCompilerAutoConfiguration
org.springframework.boot.cli.compiler.autoconfigure.SpringWebsocketCompilerAutoConfiguration
org.springframework.boot.cli.compiler.autoconfigure.TransactionManagementCompilerAutoConfiguration
org.springframework.boot.cli.compiler.dependencies.CompositeDependencyManagement
org.springframework.boot.cli.compiler.dependencies.Dependency
org.springframework.boot.cli.compiler.dependencies.Dependency.Exclusion
org.springframework.boot.cli.compiler.dependencies.DependencyManagementArtifactCoordinatesResolver
org.springframework.boot.cli.compiler.dependencies.MavenModelDependencyManagement
org.springframework.boot.cli.compiler.dependencies.SpringBootDependenciesDependencyManagement
org.springframework.boot.cli.compiler.grape.AetherGrapeEngine
org.springframework.boot.cli.compiler.grape.AetherGrapeEngineFactory
org.springframework.boot.cli.compiler.grape.CompositeProxySelector
org.springframework.boot.cli.compiler.grape.DefaultRepositorySystemSessionAutoConfiguration
org.springframework.boot.cli.compiler.grape.DependencyResolutionContext
org.springframework.boot.cli.compiler.grape.GrapeEngineInstaller
org.springframework.boot.cli.compiler.grape.GrapeRootRepositorySystemSessionAutoConfiguration
org.springframework.boot.cli.compiler.grape.RepositoryConfiguration
org.springframework.boot.cli.compiler.grape.SettingsXmlRepositorySystemSessionAutoConfiguration
org.springframework.boot.cli.compiler.maven.MavenSettings
org.springframework.boot.cli.compiler.maven.MavenSettingsReader
org.springframework.boot.cli.util.Log
org.springframework.boot.cli.util.ResourceUtils

## 异常

org.springframework.boot.cli.command.CommandException
org.springframework.boot.cli.command.NoHelpCommandArgumentsException
org.springframework.boot.cli.command.NoSuchCommandException
org.springframework.boot.cli.command.init.ReportableException
org.springframework.boot.cli.command.shell.ShellExitException
org.springframework.boot.cli.compiler.grape.DependencyResolutionFailedException






























