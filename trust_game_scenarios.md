# Trust-Game Scenario Wording

These are the trust-game stimuli used by the trust-game track.

## Investment Trust Game

- Scenario id: `investment_trust_game`
- Action schema: `trust_game`
- Tags: `trust_game`, `investment_game`, `reciprocity`

**Setup**

You are playing a one-shot investment trust game with another person. This is a single, one-time interaction; you will not meet this person again and there are no further rounds. You and the other person each have ten dollars. You decide first. You can give any whole number of dollars from 0 to 10 to the other person. Whatever you give is tripled when they receive it. They then decide how much to give back to you. Your final payment is the outcome of this single interaction.

**Reward**

both of you can end better off if you send money and the other person sends some back

**Risk**

the other person can keep the tripled money and send nothing back, leaving you worse off than if you had kept your money

**Question shown to participant**

```text
How many dollars do you give them? Answer with only the number.
```

## Investment Trust Game, repeated with fixed partner

- Scenario id: `investment_trust_game_repeated`
- Action schema: `trust_game`
- Tags: `trust_game`, `investment_game`, `reciprocity`, `repeated`

**Setup**

You are playing a repeated investment trust game with the same other person across multiple rounds. In each round, both of you start that round with the round endowment. You decide first. You can give any whole number of dollars from 0 up to your endowment. Whatever you give is tripled when they receive it. They then decide how much to give back to you. Earnings reset each round; your final payment is the sum of round outcomes.

**Reward**

both of you can end better off when you send money and the other person sends some back

**Risk**

the other person can keep the tripled money and send nothing back, leaving you worse off than if you had kept your money for that round

**Question shown to participant**

```text
How many dollars do you give them this round? Answer with only the number.
```

## Binary Betrayal Aversion Game

- Scenario id: `binary_betrayal_aversion_game`
- Action schema: `trust_game`
- Tags: `trust_game`, `betrayal_aversion`, `binary_trust`

**Setup**

You are playing a one-shot trust game. This is a single, one-time interaction; you will not meet this person again and there are no further rounds. You choose 0 or 1. If you choose 0, you and the other person each receive five dollars and the game ends. If you choose 1, the other person chooses between two outcomes: either you both receive fifteen dollars, or you receive two dollars and they receive twenty-eight dollars. Your final payment is the outcome of this single interaction.

**Reward**

if you choose 1 and the other person chooses the first outcome, you receive fifteen dollars

**Risk**

if you choose 1 and the other person chooses the second outcome, you receive two dollars

**Question shown to participant**

```text
What would you do? Answer with only 0 or 1.
```

## Moonlighting Game

- Scenario id: `moonlighting_game`
- Action schema: `trust_game`
- Tags: `trust_game`, `moonlighting`, `reciprocity`, `punishment`

**Setup**

You are playing a one-shot moonlighting trust game. This is a single, one-time interaction; you will not meet this person again and there are no further rounds. You and the other person each start with twelve talers. You move first. You can choose a number from -6 to 6. A negative number means you take that many talers from the other person for yourself. Zero means you leave the allocation unchanged. A positive number means you pass that many talers to the other person, and the amount they receive grows. Taking increases your own payoff immediately but reduces theirs. Passing costs you immediately but creates a larger surplus for them. After your move, the other person can leave things alone, reward you, or punish you even though punishment costs them too. Your final payment is the outcome of this single interaction.

**Reward**

taking talers gives you an immediate personal gain, while passing talers can create surplus and may lead to a rewarding response

**Risk**

taking talers can trigger costly punishment, while passing talers can leave you exposed if the other person does not reward you

**Question shown to participant**

```text
What would you do? Answer with only one number from -6 to 6.
```
