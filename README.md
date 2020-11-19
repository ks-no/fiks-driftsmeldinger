# fiks-driftsmeldinger

Hvis en driftsmelding er satt vil den vises som et banner på applikasjonen den er satt.

## Skjema

Driftsmeldingen må følge definisjonen i schema.json for at frontend skal vise den korrekt:

```json
{
  "message": "En feil har skjedd"
}
```

## Ny driftsmelding?

> :information_source: For at pipeline skal validere driftsmeldingene, må nye filer følge navnekonvensjonen
`{app}-fiks-{dev|test|prod}`. Husk også å oppdatere Jenkinsfile.

## Legg inn en driftsmelding

### Minside

- [Dev](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/minside-fiks-dev.json)
- [Test](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/minside-fiks-test.json)
- [Prod](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/minside-fiks-prod.json)

### Forvaltning

- [Dev](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/forvaltning-fiks-dev.json)
- [Test](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/forvaltning-fiks-test.json)
- [Prod](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/forvaltning-fiks-prod.json)

### Bekymringsmelding

- [Dev](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/bekymringsmelding-fiks-dev.json)
- [Test](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/bekymringsmelding-fiks-test.json)
- [Prod](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/bekymringsmelding-fiks-prod.json)
