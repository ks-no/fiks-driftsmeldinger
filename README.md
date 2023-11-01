
> Leter du etter driftsmeldinger for Fiks plattformen? Se [status.fiks.ks.no](https://status.fiks.ks.no).

# fiks-driftsmeldinger

Hvis en driftsmelding er satt vil den vises som et banner på applikasjonen den er satt.

## Skjema

Driftsmeldingen må følge definisjonen i schema.json for at frontend skal vise den korrekt:

```json
{
  "message": "En feil har skjedd"
}
```

## Legge inn driftsmelding for applikasjon som ikke er i listen under?

> :information_source: Ingen problem, bare lag nye filer for applikasjonen som følger navnekonvensjonen
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

### Svarut

- [Dev](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/svarut-fiks-dev.json)
- [Test](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/svarut-fiks-test.json)
- [Prod](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/svarut-fiks-prod.json)

### Covid19

- [Dev](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/dhis2-fiks-dev.json)
- [Test](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/dhis2-fiks-test.json)
- [Prod](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/dhis2-fiks-prod.json)

### Helse

- [Dev](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/helse-fiks-dev.json)
- [Test](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/helse-fiks-test.json)
- [Prod](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/helse-fiks-prod.json)

### Smittevern

- [Dev](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/smittevern-fiks-dev.json)
- [Test](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/smittevern-fiks-test.json)
- [Prod](https://github.com/ks-no/fiks-driftsmeldinger/edit/master/smittevern-fiks-prod.json)
