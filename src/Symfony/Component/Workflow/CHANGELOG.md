CHANGELOG
=========

4.0.0
-----

 * Removed class name support in `WorkflowRegistry::add()` as second parameter.

3.3.0
-----

 * Added support for expressions to guard transitions and added an `is_granted()`
   function that can be used in these expressions to use the authorization checker.
 * The `DefinitionBuilder` class now provides a fluent interface.
 * The `AuditTrailListener` now includes the workflow name in its log entries.
 * Added `workflow.entered` events which is fired after the marking has been set.
 * Deprecated class name support in `WorkflowRegistry::add()` as second parameter.
   Wrap the class name in an instance of ClassInstanceSupportStrategy instead.
 * Added support for `Event::getWorkflowName()`.
 * Added `SupportStrategyInterface` to allow custom strategies to decide whether
   or not a workflow supports a subject.
 * Added `ValidateWorkflowPass`.
