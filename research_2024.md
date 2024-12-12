## Собранный плейлист с референсами:

Плейлист:

-   https://www.youtube.com/watch?v=FQ6z90MuURM&list=PLgjfdixKuQ0o6VFBccIoWYfCdlonrlhK7&index=2&t=738s&ab_channel=CorridorCrew
-   https://www.youtube.com/playlist?list=PLgjfdixKuQ0o6VFBccIoWYfCdlonrlhK7&jct=HyhHmAy1yisdbpkdwQbsJQ

Для общего понимания того, чем мы вдохновляемся:

-   [Turn yourself into ANY STYLE with ComfyUI [PS1, 3D Animation, Anime…]](https://www.youtube.com/watch?v=efxYEbF793c&list=PLgjfdixKuQ0o6VFBccIoWYfCdlonrlhK7&index=9&ab_channel=Mickmumpitz)
-   [Create Consistent, Editable AI Characters & Backgrounds for your Projects](https://www.youtube.com/watch?v=849xBkgpF3E&list=PLgjfdixKuQ0o6VFBccIoWYfCdlonrlhK7&index=17&ab_channel=Mickmumpitz)
-   [ANIMATEDIFF COMFYUI TUTORIAL - USING CONTROLNETS AND MORE.](https://www.youtube.com/watch?v=WHxIrY2wLQE&list=PLgjfdixKuQ0o6VFBccIoWYfCdlonrlhK7&index=8&ab_channel=enigmatic_e)

## Основное, будет в использовано в workflows

Stable Diffusion и интеграция нодовой системы:

-   https://github.com/AUTOMATIC1111/stable-diffusion-webui
-   https://github.com/comfyanonymous/ComfyUI
-   https://github.com/ltdrdata/ComfyUI-Manager

Control-Net(изображение по картинке, наброску или позе) и модель для Control-Net под названием Ip-Adapter для повторения референсного стиля(изображение вместо промпта):

-   https://github.com/lllyasviel/ControlNet
-   https://journal.tinkoff.ru/controlnet/
-   https://habr.com/ru/companies/ruvds/articles/719348/
-   https://github.com/tencent-ailab/IP-Adapter
-   https://dtf.ru/howto/2235982-sozdaem-dizain-v-lyubom-stile-bez-promta-s-pomoshyu-ip-adapter

PuLID вдобавок ко всему сверху для сохранения черт лица и создания character sheets:

-   https://github.com/Mikubill/sd-webui-controlnet/discussions/2841?ysclid=m4lfr6qp4a233310366

Dreambooth для дообучения (создания кибер-Крылова):

-   https://github.com/JoePenna/Dreambooth-Stable-Diffusion
-   https://habr.com/ru/articles/760920/

VAE для улучшения качества генерации и сокращения вычислительных ресурсов:

-   https://huggingface.co/stabilityai/sd-vae-ft-mse-original
-   https://pikabu.ru/story/chto_takoe_vae_dlya_stable_diffusion_obyazatelno_dobavlyaem_9957971

Civitai, откуда будем брать модели:

-   https://pikabu.ru/story/chto_takoe_vae_dlya_stable_diffusion_obyazatelno_dobavlyaem_9957971

---

## Kaggle модели

Библиотека предварительно обученных моделей, загруженных сообществом Kaggle. Она предназначена для ускорения работы разработчиков и исследователей машинного обучения. Основные особенности раздела:

-   https://www.kaggle.com/models?task=16702&orderby=voteCount

---

## Разное

Temporal Denoising Mask Synthesis Network (TDMS-Net), предназначена для улучшения временной согласованности видео. Модель TDMS-Net решает проблему мерцания и несогласованности, возникающую при обработке видео кадр за кадром стандартными алгоритмами обработки изображений.

-   https://github.com/ZhouYiiFeng/TDMS-Net?ysclid=m41eviibux440370672

Deep Video Prior (DVP) реализация метода временной согласованности видео с использованием глубинного обучения. Предлагает подход к улучшению согласованности видео, обрабатываемого алгоритмами обработки изображений.

Повышение временной согласованности видео, обработанного такими методами, как окрашивание или удаление дымки, что позволяет преобразовать алгоритмы для изображений в алгоритмы для видео.

-   https://github.com/ChenyangLEI/deep-video-prior?tab=readme-ov-file

Проект для видео-видео синтеза на основе модели pix2pix GAN. Основная идея — преобразование видео с сохранением контента одного персонажа, но с использованием стиля другого. Реализация включает этапы предварительной обработки данных, обучения модели и постобработки для создания видео. Для работы требуются Python, GPU и CUDA. Процесс подробно описан, включая использование заранее подготовленных данных и возможность настройки параметров. Результаты сохраняются с объединением аудио и видео.

-   https://github.com/marceljmueller/vid2vid?ysclid=m41expe0bv221299258

Предоставляет конфигурации для модели FLAVR, предназначенной для интерполяции видео (добавления промежуточных кадров). Основное применение — плавное преобразование кадров для повышения качества видео. Репозиторий содержит описание структуры конфигурационных файлов, включая данные для обучения и настройки модели. Используется фреймворк PyTorch и инструменты из экосистемы MMEditing.

-   https://github.com/Libyte/mmediting/blob/main/configs/flavr/README.md?ysclid=m41f39v2es682915267

Предоставляет инструменты для локального запуска VQGAN+CLIP, модели генерации изображений из текстовых описаний. Проект основан на PyTorch, поддерживает пользовательские текстовые и стилевые подсказки, создание видео и трансформацию изображений. Включены инструкции по установке, настройке окружения, загрузке моделей и запуску генерации. Примеры показывают применение "стилевого переноса" и сюжетных генераций. Требуется GPU для оптимальной производительности.

-   https://github.com/nerdyrodent/VQGAN-CLIP

---

## Для работы с семейством моделей Stable

Модульные генеративные модели, включая text-to-video, video-to-video и text-to-video. Поддерживает настройки, тренировку, inference, а также кастомизацию моделей через YAML. Используются PyTorch Lightning и инструменты для обработки данных. Доступны примеры моделей, такие как SDXL 1.0 и Stable Video Diffusion.

-   https://github.com/Stability-AI/generative-models

-   https://github.com/nateraw/stable-diffusion-videos

---

## Материалы от Дмитрия Валерьевича Сошникова:

Перенос стиля с использованием техники Neural Style Transfer (NST).

-   https://github.com/shwars/AI_Art_Workbooks/blob/main/StyleTransfer.ipynb

-   https://github.com/shwars/AI_Art_Workbooks/blob/main/StableDiffusionWorkbook.ipynb

-   https://github.com/shwars/AI_Art_Workbooks/blob/main/StableDiffusionLatentVideo.ipynb
