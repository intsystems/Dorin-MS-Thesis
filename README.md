# Dorin-MS-Thesis

[![License](https://badgen.net/github/license/intsystems/Dorin-MS-Thesis?color=green)](https://github.com/intsystems/Dorin-MS-Thesis/blob/main/LICENSE)
[![GitHub Contributors](https://img.shields.io/github/contributors/intsystems/Dorin-MS-Thesis)](https://github.com/intsystems/Dorin-MS-Thesis/graphs/contributors)
[![GitHub Issues](https://img.shields.io/github/issues-closed/intsystems/Dorin-MS-Thesis.svg?color=0088ff)](https://github.com/intsystems/Dorin-MS-Thesis/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr-closed/intsystems/Dorin-MS-Thesis.svg?color=7f29d6)](https://github.com/intsystems/Dorin-MS-Thesis/pulls)

<table>
    <tr>
        <td align="left"> <b> Author </b> </td>
        <td> Daniil Dorin </td>
    </tr>
    <tr>
        <td align="left"> <b> Advisor </b> </td>
        <td> Andrey Grabovoy, PhD </td>
    </tr>
</table>

## Assets

- [Code](code)
- [Paper](paper/main.pdf)
- [Slides](slides/main.pdf)

## Abstract

Декодирование визуальных стимулов по нейробиологическим сигналам представляет собой ключевую задачу на стыке вычислительной нейронауки и современного машинного обучения. Несмотря на успехи, достигнутые в одномодальных подходах с применением контрастивных представлений и диффузионных генеративных моделей, большинство существующих методов опирается лишь на одну модальность~--- либо функциональную магнитно-резонансную томографию (фМРТ) с высоким пространственным разрешением, либо электроэнцефалографию (ЭЭГ) с высоким временным разрешением. Совместное использование этих модальностей остаётся слабо изученным направлением.

В работе предлагается мультимодальная архитектура, одновременно обрабатывающая записи фМРТ-ЭЭГ для реконструкции визуальных стимулов. Эмбеддинги нейробиологических сигналов обучаются контрастивно для сближения с CLIP-эмбеддингами соответствующих изображений. Двухстадийная схема генерации включает уточнение эмбеддинга мозга в CLIP-пространстве априорной диффузионной моделью и последующую генерацию изображения предобученной диффузионной моделью. Гемодинамическая задержка BOLD-сигнала анализируется через решение вспомогательной обратной задачи прогнозирования фМРТ по визуальному стимулу; полученная оценка задержки используется на этапе предобработки при формировании обучающих триплетов.

Эксперименты на открытом мультимодальном наборе данных подтверждают эффективность предложенной архитектуры в задаче нейродекодирования. По метрике CLIP-Score мультимодальная модель превосходит одномодальные аналоги, что подчёркивает необходимость совместного учёта фМРТ и ЭЭГ для точной реконструкции визуальных стимулов.

## Research Publications

1. **Dorin D.**, Kiselev N. et al. Forecasting fMRI Images From Video Sequences: Linear Model Analysis // *Health Information Science and Systems*. – 2024. [DOI: 10.1007/s13755-024-00315-5](https://doi.org/10.1007/s13755-024-00315-5)

2. **Dorin D.**, Grabovoy A., Strijov V. Enhancing fMRI Data Decoding with Spatiotemporal Characteristics in Limited Dataset // *Doklady Mathematics*. – 2025. [DOI: 10.1134/S1064562425700383](https://link.springer.com/article/10.1134/S1064562425700383)

3. **Dorin D.**, Kiselev N., Grabovoy A. Decoding Visual Information from Neural Signals: Image Reconstruction Based on Joint fMRI and EEG Analysis // *Informatika i ee Primeneniya*. – 2026.

---

## Presentations at Conferences

1. **Дорин Д.Д.**, Киселев Н.С., Грабовой А.В. Пространственно-временные методы анализа временных рядов // 66-я Всероссийская научная конференция МФТИ.

2. **Дорин Д.Д.**, Грабовой А.В. Улучшение декодирования фМРТ в условиях ограниченной выборки // 67-я Всероссийская научная конференция МФТИ.

3. **Дорин Д.Д.**, Грабовой А.В. Декодирование визуальной информации из сигналов мозга на основе пространственно-временных характеристик // 68-я Всероссийская научная конференция МФТИ.

4. **Дорин Д.Д.**, Киселев Н.С., Грабовой А.В. Декодирование визуальных стимулов из мультимодальных сигналов мозга // 22-я конференция «Математические методы распознавания образов» (ММРО-2025).

5. **Дорин Д.Д.**, Грабовой А.В. Улучшение декодирования данных фМРТ в условиях ограниченного набора данных // AI Journey 2025.

## Citation

If you find our work helpful, please cite us.
```BibTeX
@mastersthesis{dorin2026mastersthesis,
    author={Daniil Dorin},
    title={Декодирование визуальной информации из сигналов мозга на основе пространственно-временных характеристик},
    school={MIPT},
    year={2026},
    type={Master's Thesis},
    address={Moscow, Russia},
    month={June}
}
```

## Licence

Our project is MIT licensed. See [LICENSE](LICENSE) for details.
