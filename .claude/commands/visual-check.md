---
allowed-tools: mcp__playwright__browser_navigate, mcp__playwright__browser_resize, mcp__playwright__browser_take_screenshot, mcp__playwright__browser_console_messages, mcp__playwright__browser_snapshot, Read
description: Quick visual check of a page against design principles
---

Perform a quick visual verification of the specified page.

## Reference Standards

Read `/context/anti-vibe-coded-rules.md` for patterns to check.

## Process

1. Navigate to the specified URL (or localhost:3000 by default)
2. Take screenshots at:
   - Desktop (1440px)
   - Mobile (375px)
3. Check browser console for errors
4. Quick scan for vibe-coded patterns:
   - Purple gradients?
   - Sparkle overuse?
   - Aggressive hover effects?
   - Inconsistent spacing?
   - Missing loading states?
   - Broken responsive layout?

## Output

Brief report with:
- Screenshots
- Pass/Fail for vibe-coded check
- Any console errors
- Quick recommendations if issues found

**URL to check:** $ARGUMENTS (default: http://localhost:3000)
