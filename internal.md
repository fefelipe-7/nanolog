inbox {
    _index: {tipo de nota} + {data completa} + {status}
    exemplo: "inbox 02-02-2026 rascunho.md"
}

diario {
    _index: {dia da semana} + {data completa}
    exemplo: "segunda, 02-02-2026.md"
}

devaneios {
    _index: {tipo de nota} + {data completa} + {"titulo curto"}
    exemplo: "devaneio 02-02-2026 "o que é amar?".md"
}

ideias {
    _index: {tipo de nota} + {(objeto de relação)} + {data completa}
    exemplo: "ideia (presente) 02-02-2026.md"
}

memorias {
    _index: {tipo de nota} + {(objeto de memoria)} + {data completa}
    exemplo: "memoria (familia) 02-02-2026.md"
}

sonhos {
    _index: {tipo de nota} + {data completa}
    exemplo: "sonho 02-02-2026.md"
}

notas de amor {
    _index: {tipo de nota} + {index} + {"titulo curto"}
    exemplo: "nota 01: "hoje senti falta de você".md"
}

bibiloteca {
    _index: {tipo de arquivo} + {tipo de nota atrelada} + {data completa}
    exemplo: "video (devaneio) 02-02-2026.md"

    conter somente: mp3, mp4, wav, pdf, txt, docs, png, jpg
}

arquivo {
    _index: {"arquivo - "} + {antigo nome do arquivo}
    exemplo: "arquivo - inbox 02-02-2026 rascunho.md"
}