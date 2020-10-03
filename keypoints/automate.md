-   [Make][gnu-make] is a widely-used build manager.
-   A \gref{build manager}{build_manager} re-runs commands to update files that are out of date.
-   A \gref{build rule}{build_rule} has \gref{targets}{build_target}, \gref{prerequisites}{prerequisite}, and a \gref{recipe}{build_recipe}.
-   A target can be a file or a \gref{phony target}{phony_target} that simply triggers an action.
-   When a target is out of date with respect to its prerequisites, Make executes the recipe associated with its rule.
-   Make executes as many rules as it needs to when updating files, but always respects prerequisite order.
-   Make defines \gref{automatic variables}{automatic_variable} such as `$@` (target), `$^` (all prerequisites), and `$<` (first prerequisite).
-   \gref{Pattern rules}{pattern_rule} can use `%` as a placeholder for parts of filenames.
-   Makefiles can define variables using `NAME=value`.
-   Makefiles can also use functions such as `$(wildcard ...)` and `$(patsubst ...)`.
-   Use specially-formatted comments to create self-documenting Makefiles.