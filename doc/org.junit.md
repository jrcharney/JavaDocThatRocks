# JUnit

This documentation covers **JUnit 5.6.2 API**.

## Modules

This documentation consists of three sections:
* Platform
* Jupiter
* Vintage

### Platform

The **JUnit Platform** serves as a foundation for launching testing frameworks on the JVM. It also defines the **TestEngine API** for developing a testing framework that runs on the platform. Furthermore, the platform provides a **Console Launcher** to launch the platform from the command line and a JUnit 4 based **Runner** for running any TestEngine on the platform in a JUnit 4 based environment.

| Module | Description |
| :--- | :--- |
| [`org.junit.platform.commons`](org.junit.platform.commons.md) | Common APIs and support utilities for the JUnit Platform.
| [`org.junit.platform.console`](org.junit.platform.console.md) | Support for launching the JUnit Platform from the console.
| [`org.junit.platform.engine`](org.junit.platform.engine.md) | Public API for test engines.
| [`org.junit.platform.launcher`](org.junit.platform.launcher.md) | Public API for configuring and launching test plans.
| [`org.junit.platform.reporting`](org.junit.platform.reporting.md) | Defines the JUnit Platform Reporting API.
| [`org.junit.platform.runner`](org.junit.platform.runner.md) | Runner and annotations for configuring and executing tests on the JUnit Platform in a JUnit 4 environment.
| [`org.junit.platform.suite.api`](org.junit.platform.suite.api.md) | Annotations for configuring a test suite on the JUnit Platform.
| [`org.junit.platform.testkit`](org.junit.platform.testkit.md) | Defines the Test Kit API for the JUnit Platform.

### Jupiter

**JUnit Jupiter** is the combination of the new programming model and extension model for writing tests and extensions in JUnit 5. The Jupiter sub-project provides a TestEngine for running Jupiter based tests on the platform.

| Module | Description |
| :--- | :--- |
| [`org.junit.jupiter`](org.junit.jupiter.md) |	Aggregates all JUnit Jupiter modules.
| [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |	Defines JUnit Jupiter API for writing tests.
| [`org.junit.jupiter.engine`](org.junit.jupiter.engine.md) | Provides the JUnit Jupiter **`TestEngine`** implementation.
| [`org.junit.jupiter.migrationsupport`](org.junit.jupiter.migrationsupport.md) | Support for migrating from JUnit 4 to JUnit Jupiter.
| [`org.junit.jupiter.params`](org.junit.jupiter.params.md) | JUnit Jupiter extension for parameterized tests.

### Vintage

**JUnit Vintage** provides a TestEngine for running JUnit 3 and JUnit 4 based tests on the platform.

| Module | Description |
| :--- | :--- |
| [`org.junit.vintage.engine`](org.junit.vintage.engine.md) | Provides a `TestEngine` for running JUnit 3 and 4 based tests on the platform.

## All The Things!

JUnit's documentation was awesome in that they provided and entire list of classes and interfaces!

We're going to organize them a little better.

| Type | Name | Location | Description
| :--- | :--- | :--- | :--- |
| class | `AbstractTestDescriptor` | [`org.junit.platform.engine.support.descriptor`](org.junit.platform.engine.support.descriptor.md) |
| class | `AbstractTestRuleAdapter` | [`org.junit.jupiter.migrationsupport.rules.adapter`](org.junit.jupiter.migrationsupport.rules.adapter.md) |
| annotation | `AfterAll` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| interface | `AfterAllCallback` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| annotation | `AfterEach` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| interface | `AfterEachCallback` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `AfterEachMethodAdapter` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| interface | `AfterTestExecutionCallback` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| annotation | `AggregateWith` | [`org.junit.jupiter.params.aggregator`](org.junit.jupiter.params.aggregator.md) |
| interface | `AnnotationConsumer` | [`org.junit.jupiter.params.support`](org.junit.jupiter.params.support.md) |
| class | `AnnotationConsumerInitializer` | [`org.junit.jupiter.params.support`](org.junit.jupiter.params.support.md) |
| class | `AnnotationSupport` | [`org.junit.platform.commons.support`](org.junit.platform.commons.support.md) |
| class | `AnnotationUtils` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| class | `ArgumentAccessException` | [`org.junit.jupiter.params.aggregator`](org.junit.jupiter.params.aggregator.md) |
| class | `ArgumentConversionException` | [`org.junit.jupiter.params.converter`](org.junit.jupiter.params.converter.md) |
| interface | `ArgumentConverter` | [`org.junit.jupiter.params.converter`](org.junit.jupiter.params.converter.md) |
| interface | `Arguments` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| interface | `ArgumentsAccessor` | [`org.junit.jupiter.params.aggregator`](org.junit.jupiter.params.aggregator.md) |
| class | `ArgumentsAggregationException` | [`org.junit.jupiter.params.aggregator`](org.junit.jupiter.params.aggregator.md) |
| interface | `ArgumentsAggregator` | [`org.junit.jupiter.params.aggregator`](org.junit.jupiter.params.aggregator.md) |
| interface | `ArgumentsProvider` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| annotation | `ArgumentsSource` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| annotation | `ArgumentsSources` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| class | `Assertions` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `Assumptions` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| annotation | `BeforeAll` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| interface | `BeforeAllCallback` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| annotation | `BeforeEach` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| interface | `BeforeEachCallback` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `BeforeEachMethodAdapter` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| interface | `BeforeTestExecutionCallback` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| class | `BlacklistedExceptions` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| class | `CachingJupiterConfiguration` | [`org.junit.jupiter.engine.config`](org.junit.jupiter.engine.config.md) |
| class | `ClassBasedTestDescriptor` | [`org.junit.jupiter.engine.descriptor`](org.junit.jupiter.engine.descriptor.md) |
| class | `ClassFilter` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| class | `ClassLoaderUtils` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| interface | `ClassNameFilter` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| class | `ClasspathResourceSelector` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| class | `ClasspathResourceSource` | [`org.junit.platform.engine.support.descriptor`](org.junit.platform.engine.support.descriptor.md) |
| class | `ClasspathRootSelector` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| class | `ClasspathScanningSupport` | [`org.junit.platform.engine.support.filter`](org.junit.platform.engine.support.filter.md) |
| class | `ClassSelector` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| class | `ClassSource` | [`org.junit.platform.engine.support.descriptor`](org.junit.platform.engine.support.descriptor.md) |
| class | `ClassSupport` | [`org.junit.platform.commons.support`](org.junit.platform.commons.support.md) |
| class | `ClassTestDescriptor` | [`org.junit.jupiter.engine.descriptor`](org.junit.jupiter.engine.descriptor.md) |
| class | `ClassUtils` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| class | `CollectionUtils` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| class | `CommandLineOptions` | [`org.junit.platform.console.options`](org.junit.platform.console.options.md) |
| interface | `CommandLineOptionsParser` | [`org.junit.platform.console.options`](org.junit.platform.console.options.md) |
| class | `CompositeTestSource` | [`org.junit.platform.engine.support.descriptor`](org.junit.platform.engine.support.descriptor.md) |
| class | `ConditionEvaluationResult` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| class | `ConditionEvaluator` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| interface | `ConfigurationParameters` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| class | `ConsoleLauncher` | [`org.junit.platform.console`](org.junit.platform.console.md) |
| class | `ConsoleLauncherExecutionResult` | [`org.junit.platform.console`](org.junit.platform.console.md) |
| class | `ConsoleLauncherToolProvider` | [`org.junit.platform.console`](org.junit.platform.console.md) |
| class | `ConsoleTestExecutor` | [`org.junit.platform.console.tasks`](org.junit.platform.console.tasks.md) |
| class | `Constants` | [`org.junit.jupiter.engine`](org.junit.jupiter.engine.md) |
| annotation | `ConvertWith` | [`org.junit.jupiter.params.converter`](org.junit.jupiter.params.converter.md) |
| annotation | `CsvFileSource` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| class | `CsvParsingException` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| annotation | `CsvSource` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| class | `DefaultArgumentConverter` | [`org.junit.jupiter.params.converter`](org.junit.jupiter.params.converter.md) |
| class | `DefaultArgumentsAccessor` | [`org.junit.jupiter.params.aggregator`](org.junit.jupiter.params.aggregator.md) |
| class | `DefaultJupiterConfiguration` | [`org.junit.jupiter.engine.config`](org.junit.jupiter.engine.config.md) |
| enum | `DefaultParallelExecutionConfigurationStrategy` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| class | `DefaultTestInstances` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| enum | `Details` | [`org.junit.platform.console.options`](org.junit.platform.console.options.md) |
| class | `DirectorySelector` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| class | `DirectorySource` | [`org.junit.platform.engine.support.descriptor`](org.junit.platform.engine.support.descriptor.md) |
| annotation | `Disabled` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| annotation | `DisabledForJreRange` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| annotation | `DisabledIfEnvironmentVariable` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| annotation | `DisabledIfEnvironmentVariables` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| annotation | `DisabledIfSystemProperties` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| annotation | `DisabledIfSystemProperty` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| annotation | `DisabledOnJre` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| annotation | `DisabledOnOs` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| interface | `DiscoveryFilter` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| interface | `DiscoverySelector` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| class | `DiscoverySelectorResolver` | [`org.junit.jupiter.engine.discovery`](org.junit.jupiter.engine.discovery.md) |
| class | `DiscoverySelectors` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| annotation | `DisplayName` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| annotation | `DisplayNameGeneration` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| interface | `DisplayNameGenerator` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `DisplayNameGenerator.ReplaceUnderscores` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `DisplayNameGenerator.Standard` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `DynamicContainer` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `DynamicDescendantFilter` | [`org.junit.jupiter.engine.descriptor`](org.junit.jupiter.engine.descriptor.md) |
| class | `DynamicNode` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `DynamicTest` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| annotation | `EmptySource` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| annotation | `EnabledForJreRange` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| annotation | `EnabledIfEnvironmentVariable` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| annotation | `EnabledIfEnvironmentVariables` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| annotation | `EnabledIfSystemProperties` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| annotation | `EnabledIfSystemProperty` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| annotation | `EnabledOnJre` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| annotation | `EnabledOnOs` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| annotation | `EnableJUnit4MigrationSupport` | [`org.junit.jupiter.migrationsupport`](org.junit.jupiter.migrationsupport.md) |
| annotation | `EnableRuleMigrationSupport` | [`org.junit.jupiter.migrationsupport.rules`](org.junit.jupiter.migrationsupport.rules.md) |
| class | `EngineDescriptor` | [`org.junit.platform.engine.support.descriptor`](org.junit.platform.engine.support.descriptor.md) |
| interface | `EngineDiscoveryListener` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| interface | `EngineDiscoveryRequest` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| class | `EngineDiscoveryRequestResolver` | [`org.junit.platform.engine.support.discovery`](org.junit.platform.engine.support.discovery.md) |
| class | `EngineDiscoveryRequestResolver.Builder` | [`org.junit.platform.engine.support.discovery`](org.junit.platform.engine.support.discovery.md) |
| interface | `EngineDiscoveryRequestResolver.InitializationContext` | [`org.junit.platform.engine.support.discovery`](org.junit.platform.engine.support.discovery.md) |
| class | `EngineDiscoveryResult` | [`org.junit.platform.launcher`](org.junit.platform.launcher.md) |
| enum | `EngineDiscoveryResult.Status` | [`org.junit.platform.launcher`](org.junit.platform.launcher.md) |
| interface | `EngineExecutionContext` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| interface | `EngineExecutionListener` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| class | `EngineExecutionResults` | [`org.junit.platform.testkit.engine`](org.junit.platform.testkit.engine.md) |
| class | `EngineFilter` | [`org.junit.platform.launcher`](org.junit.platform.launcher.md) |
| class | `EngineTestKit` | [`org.junit.platform.testkit.engine`](org.junit.platform.testkit.engine.md) |
| class | `EngineTestKit.Builder` | [`org.junit.platform.testkit.engine`](org.junit.platform.testkit.engine.md) |
| annotation | `EnumSource` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| enum | `EnumSource.Mode` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| class | `Event` | [`org.junit.platform.testkit.engine`](org.junit.platform.testkit.engine.md) |
| class | `EventConditions` | [`org.junit.platform.testkit.engine`](org.junit.platform.testkit.engine.md) |
| class | `Events` | [`org.junit.platform.testkit.engine`](org.junit.platform.testkit.engine.md) |
| class | `EventStatistics` | [`org.junit.platform.testkit.engine`](org.junit.platform.testkit.engine.md) |
| enum | `EventType` | [`org.junit.platform.testkit.engine`](org.junit.platform.testkit.engine.md) |
| class | `ExceptionUtils` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| annotation | `ExcludeClassNamePatterns` | [`org.junit.platform.suite.api`](org.junit.platform.suite.api.md) |
| annotation | `ExcludeEngines` | [`org.junit.platform.suite.api`](org.junit.platform.suite.api.md) |
| annotation | `ExcludePackages` | [`org.junit.platform.suite.api`](org.junit.platform.suite.api.md) |
| annotation | `ExcludeTags` | [`org.junit.platform.suite.api`](org.junit.platform.suite.api.md) |
| class | `ExclusiveResource` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| enum | `ExclusiveResource.LockMode` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| interface | `Executable` | [`org.junit.jupiter.api.function`](org.junit.jupiter.api.function.md) |
| class | `ExecutableInvoker` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| interface | `ExecutableInvoker.ReflectiveInterceptorCall` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| interface | `ExecutableInvoker.ReflectiveInterceptorCall.VoidMethodInterceptorCall` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| annotation | `Execution` | [`org.junit.jupiter.api.parallel`](org.junit.jupiter.api.parallel.md) |
| class | `Execution` | [`org.junit.platform.testkit.engine`](org.junit.platform.testkit.engine.md) |
| interface | `ExecutionCondition` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| enum | `ExecutionMode` | [`org.junit.jupiter.api.parallel`](org.junit.jupiter.api.parallel.md) |
| class | `ExecutionRequest` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| class | `Executions` | [`org.junit.platform.testkit.engine`](org.junit.platform.testkit.engine.md) |
| class | `ExpectedExceptionAdapter` | [`org.junit.jupiter.migrationsupport.rules.adapter`](org.junit.jupiter.migrationsupport.rules.adapter.md) |
| class | `ExpectedExceptionSupport` | [`org.junit.jupiter.migrationsupport.rules`](org.junit.jupiter.migrationsupport.rules.md) |
| annotation | `ExtendWith` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `Extension` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| class | `ExtensionConfigurationException` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `ExtensionContext` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| class | `ExtensionContext.Namespace` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `ExtensionContext.Store` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `ExtensionContext.Store.CloseableResource` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| class | `ExtensionContextException` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `ExtensionRegistrar` | [`org.junit.jupiter.engine.extension`](org.junit.jupiter.engine.extension.md) |
| interface | `ExtensionRegistry` | [`org.junit.jupiter.engine.extension`](org.junit.jupiter.engine.extension.md) |
| annotation | `Extensions` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| class | `ExtensionValuesStore` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| class | `ExternalResourceAdapter` | [`org.junit.jupiter.migrationsupport.rules.adapter`](org.junit.jupiter.migrationsupport.rules.adapter.md) |
| class | `ExternalResourceSupport` | [`org.junit.jupiter.migrationsupport.rules`](org.junit.jupiter.migrationsupport.rules.md) |
| class | `FilePosition` | [`org.junit.platform.engine.support.descriptor`](org.junit.platform.engine.support.descriptor.md) |
| class | `FileSelector` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| class | `FileSource` | [`org.junit.platform.engine.support.descriptor`](org.junit.platform.engine.support.descriptor.md) |
| interface | `FileSystemSource` | [`org.junit.platform.engine.support.descriptor`](org.junit.platform.engine.support.descriptor.md) |
| interface | `Filter` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| interface | `Filterable` | [`org.junit.jupiter.engine.descriptor`](org.junit.jupiter.engine.descriptor.md) |
| class | `FilterResult` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| class | `ForkJoinPoolHierarchicalTestExecutorService` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| class | `FunctionUtils` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| interface | `GenericBeforeAndAfterAdvice` | [`org.junit.jupiter.migrationsupport.rules.adapter`](org.junit.jupiter.migrationsupport.rules.adapter.md) |
| class | `HierarchicalTestEngine` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| interface | `HierarchicalTestExecutorService` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| interface | `HierarchicalTestExecutorService.TestTask` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| enum | `HierarchyTraversalMode` | [`org.junit.platform.commons.support`](org.junit.platform.commons.support.md) |
| class | `IgnoreCondition` | [`org.junit.jupiter.migrationsupport.conditions`](org.junit.jupiter.migrationsupport.conditions.md) |
| annotation | `IncludeClassNamePatterns` | [`org.junit.platform.suite.api`](org.junit.platform.suite.api.md) |
| annotation | `IncludeEngines` | [`org.junit.platform.suite.api`](org.junit.platform.suite.api.md) |
| annotation | `IncludePackages` | [`org.junit.platform.suite.api`](org.junit.platform.suite.api.md) |
| annotation | `IncludeTags` | [`org.junit.platform.suite.api`](org.junit.platform.suite.api.md) |
| interface | `InvocationInterceptor` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `InvocationInterceptor.Invocation` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| class | `InvocationInterceptorChain` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| interface | `InvocationInterceptorChain.InterceptorCall` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| interface | `InvocationInterceptorChain.VoidInterceptorCall` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| class | `IsInnerClass` | [`org.junit.jupiter.engine.discovery.predicates`](org.junit.jupiter.engine.discovery.predicates.md) |
| class | `IsNestedTestClass` | [`org.junit.jupiter.engine.discovery.predicates`](org.junit.jupiter.engine.discovery.predicates.md) |
| class | `IsPotentialTestContainer` | [`org.junit.jupiter.engine.discovery.predicates`](org.junit.jupiter.engine.discovery.predicates.md) |
| class | `IsTestClassWithTests` | [`org.junit.jupiter.engine.discovery.predicates`](org.junit.jupiter.engine.discovery.predicates.md) |
| class | `IsTestFactoryMethod` | [`org.junit.jupiter.engine.discovery.predicates`](org.junit.jupiter.engine.discovery.predicates.md) |
| class | `IsTestMethod` | [`org.junit.jupiter.engine.discovery.predicates`](org.junit.jupiter.engine.discovery.predicates.md) |
| class | `IsTestTemplateMethod` | [`org.junit.jupiter.engine.discovery.predicates`](org.junit.jupiter.engine.discovery.predicates.md) |
| annotation | `JavaTimeConversionPattern` | [`org.junit.jupiter.params.converter`](org.junit.jupiter.params.converter.md) |
| enum | `JRE` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| class | `JUnitException` | [`org.junit.platform.commons`](org.junit.platform.commons.md) |
| class | `JUnitPlatform` | [`org.junit.platform.runner`](org.junit.platform.runner.md) |
| interface | `JupiterConfiguration` | [`org.junit.jupiter.engine.config`](org.junit.jupiter.engine.config.md) |
| class | `JupiterEngineDescriptor` | [`org.junit.jupiter.engine.descriptor`](org.junit.jupiter.engine.descriptor.md) |
| class | `JupiterEngineExecutionContext` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| class | `JupiterEngineExecutionContext.Builder` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| class | `JupiterTestDescriptor` | [`org.junit.jupiter.engine.descriptor`](org.junit.jupiter.engine.descriptor.md) |
| class | `JupiterTestEngine` | [`org.junit.jupiter.engine`](org.junit.jupiter.engine.md) |
| class | `JupiterThrowableCollectorFactory` | [`org.junit.jupiter.engine.support`](org.junit.jupiter.engine.support.md) |
| interface | `Launcher` | [`org.junit.platform.launcher`](org.junit.platform.launcher.md) |
| interface | `LauncherConfig` | [`org.junit.platform.launcher.core`](org.junit.platform.launcher.core.md) |
| class | `LauncherConfig.Builder` | [`org.junit.platform.launcher.core`](org.junit.platform.launcher.core.md) |
| class | `LauncherConstants` | [`org.junit.platform.launcher`](org.junit.platform.launcher.md) |
| class | `LauncherDiscoveryListener` | [`org.junit.platform.launcher`](org.junit.platform.launcher.md) |
| class | `LauncherDiscoveryListeners` | [`org.junit.platform.launcher.listeners.discovery`](org.junit.platform.launcher.listeners.discovery.md) |
| interface | `LauncherDiscoveryRequest` | [`org.junit.platform.launcher`](org.junit.platform.launcher.md) |
| class | `LauncherDiscoveryRequestBuilder` | [`org.junit.platform.launcher.core`](org.junit.platform.launcher.core.md) |
| class | `LauncherFactory` | [`org.junit.platform.launcher.core`](org.junit.platform.launcher.core.md) |
| class | `LegacyReportingUtils` | [`org.junit.platform.launcher.listeners`](org.junit.platform.launcher.listeners.md) |
| class | `LegacyReportingUtils` | [`org.junit.platform.reporting.legacy`](org.junit.platform.reporting.legacy.md) |
| class | `LegacyXmlReportGeneratingListener` | [`org.junit.platform.reporting.legacy.xml`](org.junit.platform.reporting.legacy.xml.md) |
| interface | `LifecycleMethodExecutionExceptionHandler` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `Logger` | [`org.junit.platform.commons.logging`](org.junit.platform.commons.logging.md) |
| class | `LoggerFactory` | [`org.junit.platform.commons.logging`](org.junit.platform.commons.logging.md) |
| class | `LoggingListener` | [`org.junit.platform.launcher.listeners`](org.junit.platform.launcher.listeners.md) |
| class | `LogRecordListener` | [`org.junit.platform.commons.logging`](org.junit.platform.commons.logging.md) |
| class | `LruCache` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| class | `MethodBasedTestDescriptor` | [`org.junit.jupiter.engine.descriptor`](org.junit.jupiter.engine.descriptor.md) |
| interface | `MethodDescriptor` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| interface | `MethodOrderer` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `MethodOrderer.Alphanumeric` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `MethodOrderer.OrderAnnotation` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `MethodOrderer.Random` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| interface | `MethodOrdererContext` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `MethodSelector` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| annotation | `MethodSource` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| class | `MethodSource` | [`org.junit.platform.engine.support.descriptor`](org.junit.platform.engine.support.descriptor.md) |
| class | `ModifierSupport` | [`org.junit.platform.commons.support`](org.junit.platform.commons.support.md) |
| class | `ModuleSelector` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| class | `ModuleUtils` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| class | `MutableExtensionRegistry` | [`org.junit.jupiter.engine.extension`](org.junit.jupiter.engine.extension.md) |
| class | `NamespaceAwareStore` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| annotation | `Nested` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `NestedClassSelector` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| class | `NestedClassTestDescriptor` | [`org.junit.jupiter.engine.descriptor`](org.junit.jupiter.engine.descriptor.md) |
| class | `NestedMethodSelector` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| interface | `Node` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| interface | `Node.DynamicTestExecutor` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| enum | `Node.ExecutionMode` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| interface | `Node.Invocation` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| class | `Node.SkipResult` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| annotation | `NullAndEmptySource` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| enum | `NullEnum` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| annotation | `NullSource` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| class | `OpenTest4JAwareThrowableCollector` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| annotation | `Order` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| enum | `OS` | [`org.junit.jupiter.api.condition`](org.junit.jupiter.api.condition.md) |
| interface | `PackageNameFilter` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| class | `PackageSelector` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| class | `PackageSource` | [`org.junit.platform.engine.support.descriptor`](org.junit.platform.engine.support.descriptor.md) |
| class | `PackageUtils` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| interface | `ParallelExecutionConfiguration` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| interface | `ParallelExecutionConfigurationStrategy` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| interface | `ParameterContext` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| annotation | `ParameterizedTest` | [`org.junit.jupiter.params`](org.junit.jupiter.params.md) |
| class | `ParameterResolutionException` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `ParameterResolver` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `ParseResult` | [`org.junit.platform.launcher.tagexpression`](org.junit.platform.launcher.tagexpression.md) |
| class | `PicocliCommandLineOptionsParser` | [`org.junit.platform.console.options`](org.junit.platform.console.options.md) |
| interface | `PostDiscoveryFilter` | [`org.junit.platform.launcher`](org.junit.platform.launcher.md) |
| class | `Preconditions` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| class | `PreconditionViolationException` | [`org.junit.platform.commons`](org.junit.platform.commons.md) |
| class | `PreconditionViolationException` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| class | `PrefixedConfigurationParameters` | [`org.junit.platform.engine.support.config`](org.junit.platform.engine.support.config.md) |
| class | `ReflectionSupport` | [`org.junit.platform.commons.support`](org.junit.platform.commons.support.md) |
| class | `ReflectionUtils` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| enum | `ReflectionUtils.HierarchyTraversalMode` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| interface | `ReflectiveInvocationContext` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| annotation | `RegisterExtension` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| annotation | `RepeatedTest` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| interface | `RepetitionInfo` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `ReportEntry` | [`org.junit.platform.engine.reporting`](org.junit.platform.engine.reporting.md) |
| enum | `ResourceAccessMode` | [`org.junit.jupiter.api.parallel`](org.junit.jupiter.api.parallel.md) |
| annotation | `ResourceLock` | [`org.junit.jupiter.api.parallel`](org.junit.jupiter.api.parallel.md) |
| interface | `ResourceLock` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| annotation | `ResourceLocks` | [`org.junit.jupiter.api.parallel`](org.junit.jupiter.api.parallel.md) |
| class | `Resources` | [`org.junit.jupiter.api.parallel`](org.junit.jupiter.api.parallel.md) |
| interface | `RunnerDecorator` | [`org.junit.vintage.engine.descriptor`](org.junit.vintage.engine.descriptor.md) |
| class | `RunnerExecutor` | [`org.junit.vintage.engine.execution`](org.junit.vintage.engine.execution.md) |
| class | `RunnerTestDescriptor` | [`org.junit.vintage.engine.descriptor`](org.junit.vintage.engine.descriptor.md) |
| class | `RuntimeUtils` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| class | `SameThreadHierarchicalTestExecutorService` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| annotation | `SelectClasses` | [`org.junit.platform.suite.api`](org.junit.platform.suite.api.md) |
| class | `SelectorResolutionResult` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| enum | `SelectorResolutionResult.Status` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| interface | `SelectorResolver` | [`org.junit.platform.engine.support.discovery`](org.junit.platform.engine.support.discovery.md) |
| interface | `SelectorResolver.Context` | [`org.junit.platform.engine.support.discovery`](org.junit.platform.engine.support.discovery.md) |
| class | `SelectorResolver.Match` | [`org.junit.platform.engine.support.discovery`](org.junit.platform.engine.support.discovery.md) |
| class | `SelectorResolver.Resolution` | [`org.junit.platform.engine.support.discovery`](org.junit.platform.engine.support.discovery.md) |
| annotation | `SelectPackages` | [`org.junit.platform.suite.api`](org.junit.platform.suite.api.md) |
| class | `SimpleArgumentConverter` | [`org.junit.jupiter.params.converter`](org.junit.jupiter.params.converter.md) |
| class | `SingleTestExecutor` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| interface | `SingleTestExecutor.Executable` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| class | `StringUtils` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| annotation | `SuiteDisplayName` | [`org.junit.platform.suite.api`](org.junit.platform.suite.api.md) |
| class | `SummaryGeneratingListener` | [`org.junit.platform.launcher.listeners`](org.junit.platform.launcher.listeners.md) |
| annotation | `Tag` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| interface | `TagExpression` | [`org.junit.platform.launcher.tagexpression`](org.junit.platform.launcher.tagexpression.md) |
| class | `TagFilter` | [`org.junit.platform.launcher`](org.junit.platform.launcher.md) |
| annotation | `Tags` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| annotation | `TempDir` | [`org.junit.jupiter.api.io`](org.junit.jupiter.api.io.md) |
| class | `TerminationInfo` | [`org.junit.platform.testkit.engine`](org.junit.platform.testkit.engine.md) |
| annotation | `Test` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| annotation | `Testable` | [`org.junit.platform.commons.annotation`](org.junit.platform.commons.annotation.md) |
| interface | `TestDescriptor` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| enum | `TestDescriptor.Type` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| interface | `TestDescriptor.Visitor` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| interface | `TestEngine` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| interface | `TestExecutionExceptionHandler` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `TestExecutionListener` | [`org.junit.platform.launcher`](org.junit.platform.launcher.md) |
| class | `TestExecutionResult` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| enum | `TestExecutionResult.Status` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| class | `TestExecutionResultConditions` | [`org.junit.platform.testkit.engine`](org.junit.platform.testkit.engine.md) |
| interface | `TestExecutionSummary` | [`org.junit.platform.launcher.listeners`](org.junit.platform.launcher.listeners.md) |
| interface | `TestExecutionSummary.Failure` | [`org.junit.platform.launcher.listeners`](org.junit.platform.launcher.listeners.md) |
| annotation | `TestFactory` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `TestFactoryTestDescriptor` | [`org.junit.jupiter.engine.descriptor`](org.junit.jupiter.engine.descriptor.md) |
| class | `TestIdentifier` | [`org.junit.platform.launcher`](org.junit.platform.launcher.md) |
| interface | `TestInfo` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| annotation | `TestInstance` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| enum | `TestInstance.Lifecycle` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| interface | `TestInstanceFactory` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `TestInstanceFactoryContext` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| class | `TestInstanceLifecycleUtils` | [`org.junit.jupiter.engine.descriptor`](org.junit.jupiter.engine.descriptor.md) |
| interface | `TestInstancePostProcessor` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `TestInstancePreDestroyCallback` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `TestInstances` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `TestInstancesProvider` | [`org.junit.jupiter.engine.execution`](org.junit.jupiter.engine.execution.md) |
| class | `TestInstantiationException` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| annotation | `TestMethodOrder` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `TestMethodTestDescriptor` | [`org.junit.jupiter.engine.descriptor`](org.junit.jupiter.engine.descriptor.md) |
| class | `TestPlan` | [`org.junit.platform.launcher`](org.junit.platform.launcher.md) |
| interface | `TestReporter` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `TestRuleAnnotatedField` | [`org.junit.jupiter.migrationsupport.rules.member`](org.junit.jupiter.migrationsupport.rules.member.md) |
| interface | `TestRuleAnnotatedMember` | [`org.junit.jupiter.migrationsupport.rules.member`](org.junit.jupiter.migrationsupport.rules.member.md) |
| class | `TestRuleAnnotatedMethod` | [`org.junit.jupiter.migrationsupport.rules.member`](org.junit.jupiter.migrationsupport.rules.member.md) |
| interface | `TestSource` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| class | `TestSourceProvider` | [`org.junit.vintage.engine.descriptor`](org.junit.vintage.engine.descriptor.md) |
| class | `TestTag` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| annotation | `TestTemplate` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| interface | `TestTemplateInvocationContext` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| interface | `TestTemplateInvocationContextProvider` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| class | `TestTemplateInvocationTestDescriptor` | [`org.junit.jupiter.engine.descriptor`](org.junit.jupiter.engine.descriptor.md) |
| class | `TestTemplateTestDescriptor` | [`org.junit.jupiter.engine.descriptor`](org.junit.jupiter.engine.descriptor.md) |
| interface | `TestWatcher` | [`org.junit.jupiter.api.extension`](org.junit.jupiter.api.extension.md) |
| enum | `Theme` | [`org.junit.platform.console.options`](org.junit.platform.console.options.md) |
| class | `ThrowableCollector` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| interface | `ThrowableCollector.Executable` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| interface | `ThrowableCollector.Factory` | [`org.junit.platform.engine.support.hierarchical`](org.junit.platform.engine.support.hierarchical.md) |
| interface | `ThrowingConsumer` | [`org.junit.jupiter.api.function`](org.junit.jupiter.api.function.md) |
| interface | `ThrowingSupplier` | [`org.junit.jupiter.api.function`](org.junit.jupiter.api.function.md) |
| annotation | `Timeout` | [`org.junit.jupiter.api`](org.junit.jupiter.api.md) |
| class | `ToStringBuilder` | [`org.junit.platform.commons.util`](org.junit.platform.commons.util.md) |
| class | `Try` | [`org.junit.platform.commons.function`](org.junit.platform.commons.function.md) |
| interface | `Try.Transformer` | [`org.junit.platform.commons.function`](org.junit.platform.commons.function.md) |
| class | `TypeBasedParameterResolver` | [`org.junit.jupiter.api.extension.support`](org.junit.jupiter.api.extension.support.md) |
| class | `UniqueId` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| class | `UniqueId.Segment` | [`org.junit.platform.engine`](org.junit.platform.engine.md) |
| class | `UniqueIdReader` | [`org.junit.vintage.engine.support`](org.junit.vintage.engine.support.md) |
| class | `UniqueIdSelector` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| class | `UniqueIdStringifier` | [`org.junit.vintage.engine.support`](org.junit.vintage.engine.support.md) |
| class | `UriSelector` | [`org.junit.platform.engine.discovery`](org.junit.platform.engine.discovery.md) |
| interface | `UriSource` | [`org.junit.platform.engine.support.descriptor`](org.junit.platform.engine.support.descriptor.md) |
| annotation | `UseTechnicalNames` | [`org.junit.platform.suite.api`](org.junit.platform.suite.api.md) |
| annotation | `ValueSource` | [`org.junit.jupiter.params.provider`](org.junit.jupiter.params.provider.md) |
| class | `VerifierAdapter` | [`org.junit.jupiter.migrationsupport.rules.adapter`](org.junit.jupiter.migrationsupport.rules.adapter.md) |
| class | `VerifierSupport` | [`org.junit.jupiter.migrationsupport.rules`](org.junit.jupiter.migrationsupport.rules.md) |
| class | `VintageDiscoverer` | [`org.junit.vintage.engine.discovery`](org.junit.vintage.engine.discovery.md) |
| class | `VintageEngineDescriptor` | [`org.junit.vintage.engine.descriptor`](org.junit.vintage.engine.descriptor.md) |
| class | `VintageTestDescriptor` | [`org.junit.vintage.engine.descriptor`](org.junit.vintage.engine.descriptor.md) |
| class | `VintageTestEngine` | [`org.junit.vintage.engine`](org.junit.vintage.engine.md) |


## Sources
* JUnit. [JUnit 5.6.2 API](https://junit.org/junit5/docs/current/api/). 18 May 2020.
* JUnit. [All Classes (JUnit 5.6.2 API)](https://junit.org/junit5/docs/current/api/allclasses.html). 18 May 2020.