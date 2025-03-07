# Roo Code Changelog

## [3.3.2]

- Add a dropdown to select the API configuration for a mode in the Prompts tab
- Fix bug where always allow wasn't showing up for MCP tools
- Improve OpenRouter DeepSeek-R1 integration by setting temperature to the recommended 0.6 and displaying the reasoning output (thanks @Szpadel - it's really fascinating to watch!)
- Allow specifying a custom OpenRouter base URL (thanks @dairui1!)
- Make the UI for nested settings nicer (thanks @PretzelVector!)

## [3.3.1]

- Fix issue where the terminal management system was creating unnecessary new terminals (thanks @evan-fannin!)
- Fix bug where the saved API provider for a mode wasn't being selected after a mode switch command

## [3.3.0]

- Native VS Code code actions support with quick fixes and refactoring options
- Modes can now request to switch to other modes when needed
- Ask and Architect modes can now edit markdown files
- Custom modes can now be restricted to specific file patterns (for example, a technical writer who can only edit markdown files 👋)
- Support for configuring the Bedrock provider with AWS Profiles
- New Roo Code community Discord at https://roocode.com/discord!

## [3.2.8]

- Fixed bug opening custom modes settings JSON
- Reverts provider key entry back to checking onInput instead of onChange to hopefully address issues entering API keys (thanks @samhvw8!)
- Added explicit checkbox to use Azure for OpenAI compatible providers (thanks @samhvw8!)
- Fixed Glama usage reporting (thanks @punkpeye!)
- Added Llama 3.3 70B Instruct model to the AWS Bedrock provider options (thanks @Premshay!)

## [3.2.7]

- Fix bug creating new configuration profiles

## [3.2.6]

- Fix bug with role definition overrides for built-in modes

## [3.2.5]

- Added gemini flash thinking 01-21 model and a few visual fixes (thanks @monotykamary!)

## [3.2.4]

- Only allow use of the diff tool if it's enabled in settings

## [3.2.3]

- Fix bug where language selector wasn't working

## [3.2.0 - 3.2.2]

- **Name Change From Roo Cline to Roo Code:** We're excited to announce our new name! After growing beyond 50,000 installations, we've rebranded from Roo Cline to Roo Code to better reflect our identity as we chart our own course.

- **Custom Modes:** Create your own personas for Roo Code! While our built-in modes (Code, Architect, Ask) are still here, you can now shape entirely new ones:
    - Define custom prompts
    - Choose which tools each mode can access
    - Create specialized assistants for any workflow
    - Just type "Create a new mode for <X>" or visit the Prompts tab in the top menu to get started

Join us at https://www.reddit.com/r/RooCode to share your custom modes and be part of our next chapter!

## [3.1.7]

- DeepSeek-R1 support (thanks @philipnext!)
- Experimental new unified diff algorithm can be enabled in settings (thanks @daniel-lxs!)
- More fixes to configuration profiles (thanks @samhvw8!)

## [3.1.6]

- Add Mistral (thanks Cline!)
- Fix bug with VSCode LM configuration profile saving (thanks @samhvw8!)

## [3.1.4 - 3.1.5]

- Bug fixes to the auto approve menu

## [3.1.3]

- Add auto-approve chat bar (thanks Cline!)
- Fix bug with VS Code Language Models integration

## [3.1.2]

- Experimental support for VS Code Language Models including Copilot (thanks @RaySinner / @julesmons!)
- Fix bug related to configuration profile switching (thanks @samhvw8!)
- Improvements to fuzzy search in mentions, history, and model lists (thanks @samhvw8!)
- PKCE support for Glama (thanks @punkpeye!)
- Use 'developer' message for o1 system prompt

## [3.1.1]

- Visual fixes to chat input and settings for the light+ themes

## [3.1.0]

- You can now customize the role definition and instructions for each chat mode (Code, Architect, and Ask), either through the new Prompts tab in the top menu or mode-specific .clinerules-mode files. Prompt Enhancements have also been revamped: the "Enhance Prompt" button now works with any provider and API configuration, giving you the ability to craft messages with fully customizable prompts for even better results.
- Add a button to copy markdown out of the chat

## [3.0.3]

- Update required vscode engine to ^1.84.0 to match cline

## [3.0.2]

- A couple more tiny tweaks to the button alignment in the chat input

## [3.0.1]

- Fix the reddit link and a small visual glitch in the chat input

## [3.0.0]

- This release adds chat modes! Now you can ask Roo Code questions about system architecture or the codebase without immediately jumping into writing code. You can even assign different API configuration profiles to each mode if you prefer to use different models for thinking vs coding. Would love feedback in the new Roo Code Reddit! https://www.reddit.com/r/RooCode

## [2.2.46]

- Only parse @-mentions in user input (not in files)

## [2.2.45]

- Save different API configurations to quickly switch between providers and settings (thanks @samhvw8!)

## [2.2.44]

- Automatically retry failed API requests with a configurable delay (thanks @RaySinner!)

## [2.2.43]

- Allow deleting single messages or all subsequent messages

## [2.2.42]

- Add a Git section to the context mentions

## [2.2.41]

- Checkbox to disable streaming for OpenAI-compatible providers

## [2.2.40]

- Add the Glama provider (thanks @punkpeye!)

## [2.2.39]

- Add toggle to enable/disable the MCP-related sections of the system prompt (thanks @daniel-lxs!)

## [2.2.38]

- Add a setting to control the number of terminal output lines to pass to the model when executing commands

## [2.2.36 - 2.2.37]

- Add a button to delete user messages

## [2.2.35]

- Allow selection of multiple browser viewport sizes and adjusting screenshot quality

## [2.2.34]

- Add the DeepSeek provider

## [2.2.33]

- "Enhance prompt" button (OpenRouter models only for now)
- Support listing models for OpenAI compatible providers (thanks @samhvw8!)

## [2.2.32]

- More efficient workspace tracker

## [2.2.31]

- Improved logic for auto-approving chained commands

## [2.2.30]

- Fix bug with auto-approving commands

## [2.2.29]

- Add configurable delay after auto-writes to allow diagnostics to catch up

## [2.2.28]

- Use createFileSystemWatcher to more reliably update list of files to @-mention

## [2.2.27]

- Add the current time to the system prompt and improve browser screenshot quality (thanks @libertyteeth!)

## [2.2.26]

- Tweaks to preferred language (thanks @yongjer)

## [2.2.25]

- Add a preferred language dropdown

## [2.2.24]

- Default diff editing to on for new installs

## [2.2.23]

- Fix context window for gemini-2.0-flash-thinking-exp-1219 (thanks @student20880)

## [2.2.22]

- Add gemini-2.0-flash-thinking-exp-1219

## [2.2.21]

- Take predicted file length into account when detecting omissions

## [2.2.20]

- Make fuzzy diff matching configurable (and default to off)

## [2.2.19]

- Add experimental option to use a bigger browser (1280x800)

## [2.2.18]

- More targeted styling fix for Gemini chats

## [2.2.17]

- Improved regex for auto-execution of chained commands

## [2.2.16]

- Incorporate Premshay's [PR](https://github.com/RooVetGit/Roo-Cline/pull/60) to add support for Amazon Nova and Meta Llama Models via Bedrock (3, 3.1, 3.2) and unified Bedrock calls using BedrockClient and Bedrock Runtime API

## [2.2.14 - 2.2.15]

- Make diff editing more robust to transient errors / fix bugs

## [2.2.13]

- Fixes to sound playing and applying diffs

## [2.2.12]

- Better support for pure deletion and insertion diffs

## [2.2.11]

- Added settings checkbox for verbose diff debugging

## [2.2.6 - 2.2.10]

- More fixes to search/replace diffs

## [2.2.5]

- Allow MCP servers to be enabled/disabled

## [2.2.4]

- Tweak the prompt to encourage diff edits when they're enabled

## [2.2.3]

- Clean up the settings screen

## [2.2.2]

- Add checkboxes to auto-approve MCP tools

## [2.2.1]

- Fix another diff editing indentation bug

## [2.2.0]

- Incorporate MCP changes from Cline 2.2.0

## [2.1.21]

- Larger text area input + ability to drag images into it

## [2.1.20]

- Add Gemini 2.0

## [2.1.19]

- Better error handling for diff editing

## [2.1.18]

- Diff editing bugfix to handle Windows line endings

## [2.1.17]

- Switch to search/replace diffs in experimental diff editing mode

## [2.1.16]

- Allow copying prompts from the history screen

## [2.1.15]

- Incorporate dbasclpy's [PR](https://github.com/RooVetGit/Roo-Cline/pull/54) to add support for gemini-exp-1206
- Make it clear that diff editing is very experimental

## [2.1.14]

- Fix bug where diffs were not being applied correctly and try Aider's [unified diff prompt](https://github.com/Aider-AI/aider/blob/3995accd0ca71cea90ef76d516837f8c2731b9fe/aider/coders/udiff_prompts.py#L75-L105)
- If diffs are enabled, automatically reject write_to_file commands that lead to truncated output

## [2.1.13]

- Fix https://github.com/RooVetGit/Roo-Cline/issues/50 where sound effects were not respecting settings

## [2.1.12]

- Incorporate JoziGila's [PR](https://github.com/cline/cline/pull/158) to add support for editing through diffs

## [2.1.11]

- Incorporate lloydchang's [PR](https://github.com/RooVetGit/Roo-Cline/pull/42) to add support for OpenRouter compression

## [2.1.10]

- Incorporate HeavenOSK's [PR](https://github.com/cline/cline/pull/818) to add sound effects to Cline

## [2.1.9]

- Add instructions for using .clinerules on the settings screen

## [2.1.8]

- Roo Cline now allows configuration of which commands are allowed without approval!

## [2.1.7]

- Updated extension icon and metadata

## [2.2.0]

- Add support for Model Context Protocol (MCP), enabling Cline to use custom tools like web-search tool or GitHub tool
- Add MCP server management tab accessible via the server icon in the menu bar
- Add ability for Cline to dynamically create new MCP servers based on user requests (e.g., "add a tool that gets the latest npm docs")

## [2.1.6]

- Roo Cline now runs in all VSCode-compatible editors

## [2.1.5]

- Fix bug in browser action approval

## [2.1.4]

- Roo Cline now can run side-by-side with Cline

## [2.1.3]

- Roo Cline now allows browser actions without approval when `alwaysAllowBrowser` is true

## [2.1.2]

- Support for auto-approval of write operations and command execution
- Support for .clinerules custom instructions
