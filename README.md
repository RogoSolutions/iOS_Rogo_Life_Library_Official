Release Note

Version 1.0.9.5:
- Update function addSmartAutomation
 // MARK: - New smart automation
    /**
     * Adds a new smart automation. The process can include up to 3 steps:
     * 1. Creating a smart automation (mandatory).
     * 2. Adding triggers to the smart automation (optional).
     * 3. Adding commands to the smart automation (optional).
     *
     * - The `initSmartCompletionHandler` is called after the smart creation step, whether it succeeds or fails.
     * - The `addTriggerCompletionHandler` is called for each trigger addition step, whether it succeeds or fails.
     * - The `addCommandCompletionHandler` is called for each command addition step, whether it succeeds or fails.
     * - The `completion` callback is invoked after all steps have been completed.
     *
     * If `failOnTriggerError` is true, the `completion` callback will report failure if any trigger addition fails.
     * If `failOnCommandError` is true, the `completion` callback will report failure if any command addition fails.
     *
     * - Parameters:
     *   - smartTitle: The title for the smart automation.
     *   - automationType: The type of automation to create.
     *   - triggers: A list of triggers to associate with the smart automation.
     *   - commands: A list of commands to execute within the smart automation.
     *   - failOnTriggerError: A flag indicating whether the process should fail if any trigger addition fails.
     *   - failOnCommandError: A flag indicating whether the process should fail if any command addition fails.
     *   - initSmartCompletionHandler: Callback invoked after the smart creation step.
     *   - addTriggerCompletionHandler: Callback invoked for each trigger addition step.
     *   - addCommandCompletionHandler: Callback invoked for each command addition step, providing the index, response, and error.
     *   - completion: Final callback invoked after all steps have been completed.
     */

