# Review surface routing evaluation

## Question

Which Commentary surface should a support agent recommend?

## Expected answers

- Generated HTML reports use Static HTML Review.
- Interactive preview apps use Live Preview Review.
- Pre-Git documents use Draft Review.
- Consensus-building plans use Brainstorming Review.
- Markdown files in public or private PRs use rendered Markdown PR review.
- Branch documents that are not ready for a PR use direct document review.

## Regression prompts

1. A customer has an exported compliance report with tables and inline CSS. Recommend Static HTML Review and mention sandboxed active content.
2. A design partner wants to comment on a billing button in a staging app. Recommend Live Preview Review and mention SDK opt-in plus frameability.
3. A support lead has a memo in Slack that has not been committed. Recommend Draft Review.
4. An agent needs to propose changes to a rollout plan with objections and owner decisions. Recommend Brainstorming Review.
