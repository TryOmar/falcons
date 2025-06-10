# Software Developer – Lua Questions & Answers

Each question is labeled (e.g., `L4 - 27`) and includes both the original code (possibly with mistakes) and the corrected version.

---

## L4 - 27

### Question

~~~lua
function kickAFKPlayers()
    for i, player in ipairs(getElementsByType("player")) do
        local lastMove = getElementData("lastMoveTime") -- Forgot to specify the player.
        if (lastMove and getTickCount() - lastMove > 300000) then -- Make it only kick logged in players using isGuestAccount and getPlayerAccount inside it.
            kickPlayer(player, "AFK too long")
        end
    end
end

-- A developer tried to kick AFK players but made multiple mistakes.
-- Hint: Ensure the player is logged in.
-- Check if the account isn't a guest one, and getPlayerAccount(argument).
~~~

### Answer

~~~lua
function kickAFKPlayers()
    for i, player in ipairs(getElementsByType("player")) do
        local lastMove = getElementData(player, "lastMoveTime")
        if (lastMove and getTickCount() - lastMove > 300000 and not isGuestAccount(getPlayerAccount(player))) then
            kickPlayer(player, "AFK too long")
        end
    end
end
~~~

---

## L4 - XX

### Question

~~~lua
-- Add your next question here.
-- Replace XX with the proper number (e.g., 28, 29).
-- Include the code and hints if any.
~~~

### Answer

~~~lua
-- Provide the corrected or ideal solution here.
~~~

---
