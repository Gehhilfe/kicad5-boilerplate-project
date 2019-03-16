# kicad5-boilerplate-project

1. Fork this repo
2. Checkout repo
3. Configure smudge and clean filters to remove diff noise

```
git config --local filter.kicad_project.clean "sed -E 's/^update=.*$/update=Date/'"
git config --local filter.kicad_project.smudge cat
git config --local filter.kicad_sch.clean "sed -E 's/#(PWR|FLG)[0-9]+/#\1?/'"
git config --local filter.kicad_sch.smudge cat
```

Have Fun!
