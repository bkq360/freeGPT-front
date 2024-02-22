<script setup>

</script>
<template>
  <div class="left-main">
    <div class="main-layout">
      <div>
        <div class="flex mb-6 flex-row-reverse">
          <div class="item-content ml-2 basis-8 flex items-center flex-shrink-0 h-8 justify-center">
            <span class="text-icon">
              <img src="/public/user.jpg" width="34px">
            </span>
          </div>
          <div class="text-sm">
            <p class="text-xs text-right">2024/1/27 12:38:00</p>
            <div class="flex item-end mt-2 flex-row-reverse gap-1">
              <div class="text-black bg-user min-w px-3 py-2 rounded-md">
                <div class="mkdown-body">
                  <p>
                    flex-basis 是 CSS 中 Flexbox 布局模型的一个属性。它用于设置伸缩项目的初始主轴尺寸。可以指定一个固定的长度值?
                  </p>
                </div>
              </div>
              <div class="flex flex-col">
                <button class="transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-200">
                  <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M12 3c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0 14c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0-7c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2">
                    </path>
                  </svg>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="flex mb-6 flex-row">
          <div class="item-content mr-2 basis-8 flex items-center flex-shrink-0 h-8 justify-center">
            <span class="text-icon">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32" aria-hidden="true" width="1em" height="1em">
                <path
                  d="M29.71,13.09A8.09,8.09,0,0,0,20.34,2.68a8.08,8.08,0,0,0-13.7,2.9A8.08,8.08,0,0,0,2.3,18.9,8,8,0,0,0,3,25.45a8.08,8.08,0,0,0,8.69,3.87,8,8,0,0,0,6,2.68,8.09,8.09,0,0,0,7.7-5.61,8,8,0,0,0,5.33-3.86A8.09,8.09,0,0,0,29.71,13.09Zm-12,16.82a6,6,0,0,1-3.84-1.39l.19-.11,6.37-3.68a1,1,0,0,0,.53-.91v-9l2.69,1.56a.08.08,0,0,1,.05.07v7.44A6,6,0,0,1,17.68,29.91ZM4.8,24.41a6,6,0,0,1-.71-4l.19.11,6.37,3.68a1,1,0,0,0,1,0l7.79-4.49V22.8a.09.09,0,0,1,0,.08L13,26.6A6,6,0,0,1,4.8,24.41ZM3.12,10.53A6,6,0,0,1,6.28,7.9v7.57a1,1,0,0,0,.51.9l7.75,4.47L11.85,22.4a.14.14,0,0,1-.09,0L5.32,18.68a6,6,0,0,1-2.2-8.18Zm22.13,5.14-7.78-4.52L20.16,9.6a.08.08,0,0,1,.09,0l6.44,3.72a6,6,0,0,1-.9,10.81V16.56A1.06,1.06,0,0,0,25.25,15.67Zm2.68-4-.19-.12-6.36-3.7a1,1,0,0,0-1.05,0l-7.78,4.49V9.2a.09.09,0,0,1,0-.09L19,5.4a6,6,0,0,1,8.91,6.21ZM11.08,17.15,8.38,15.6a.14.14,0,0,1-.05-.08V8.1a6,6,0,0,1,9.84-4.61L18,3.6,11.61,7.28a1,1,0,0,0-.53.91ZM12.54,14,16,12l3.47,2v4L16,20l-3.47-2Z"
                  fill="currentColor"></path>
              </svg>
            </span>
          </div>
          <div class="text-sm">
            <p class="text-xs text-left">2024/1/27 12:38:00</p>
            <div class="flex item-end mt-2 flex-row gap-1">
              <div class="text-black bg-system min-w px-3 py-2 rounded-md">
                <div class="mkdown-body">
                  <p>
                    flex-basis 是 CSS 中 Flexbox 布局模型的一个属性。它用于设置伸缩项目的初始主轴尺寸。可以指定一个固定的长度值，比如 flex-basis: 300px;，或者使用相对值，比如
                    flex-basis: 50%;。这个属性通常与 flex-grow 和 flex-shrink 属性一起使用来控制伸缩项目在 Flex 容器中的布局行为。
                  </p>
                </div>
              </div>
              <div class="flex flex-col">
                <button class="mb-2 transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-300">
                  <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M18.537 19.567A9.961 9.961 0 0 1 12 22C6.477 22 2 17.523 2 12S6.477 2 12 2s10 4.477 10 10c0 2.136-.67 4.116-1.81 5.74L17 12h3a8 8 0 1 0-2.46 5.772z">
                    </path>
                  </svg></button><button
                  class="transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-200">
                  <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M12 3c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0 14c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0-7c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2">
                    </path>
                  </svg>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="flex mb-6 flex-row-reverse">
          <div class="item-content ml-2 basis-8 flex items-center flex-shrink-0 h-8 justify-center">
            <span class="text-icon">
              <img src="/public/user.jpg" width="34px">
            </span>
          </div>
          <div class="text-sm">
            <p class="text-xs text-right">2024/1/27 12:38:00</p>
            <div class="flex item-end mt-2 flex-row-reverse gap-1">
              <div class="text-black bg-user min-w px-3 py-2 rounded-md">
                <div class="mkdown-body">
                  <p>
                    flex-basis 是 CSS 中 Flexbox 布局模型的一个属性。它用于设置伸缩项目的初始主轴尺寸。可以指定一个固定的长度值?
                  </p>
                </div>
              </div>
              <div class="flex flex-col">
                <button class="transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-200">
                    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M12 3c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0 14c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0-7c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2">
                    </path>
                  </svg>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="flex mb-6 flex-row">
          <div class="item-content mr-2 basis-8 flex items-center flex-shrink-0 h-8 justify-center">
            <span class="text-icon">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32" aria-hidden="true" width="1em" height="1em">
                <path
                  d="M29.71,13.09A8.09,8.09,0,0,0,20.34,2.68a8.08,8.08,0,0,0-13.7,2.9A8.08,8.08,0,0,0,2.3,18.9,8,8,0,0,0,3,25.45a8.08,8.08,0,0,0,8.69,3.87,8,8,0,0,0,6,2.68,8.09,8.09,0,0,0,7.7-5.61,8,8,0,0,0,5.33-3.86A8.09,8.09,0,0,0,29.71,13.09Zm-12,16.82a6,6,0,0,1-3.84-1.39l.19-.11,6.37-3.68a1,1,0,0,0,.53-.91v-9l2.69,1.56a.08.08,0,0,1,.05.07v7.44A6,6,0,0,1,17.68,29.91ZM4.8,24.41a6,6,0,0,1-.71-4l.19.11,6.37,3.68a1,1,0,0,0,1,0l7.79-4.49V22.8a.09.09,0,0,1,0,.08L13,26.6A6,6,0,0,1,4.8,24.41ZM3.12,10.53A6,6,0,0,1,6.28,7.9v7.57a1,1,0,0,0,.51.9l7.75,4.47L11.85,22.4a.14.14,0,0,1-.09,0L5.32,18.68a6,6,0,0,1-2.2-8.18Zm22.13,5.14-7.78-4.52L20.16,9.6a.08.08,0,0,1,.09,0l6.44,3.72a6,6,0,0,1-.9,10.81V16.56A1.06,1.06,0,0,0,25.25,15.67Zm2.68-4-.19-.12-6.36-3.7a1,1,0,0,0-1.05,0l-7.78,4.49V9.2a.09.09,0,0,1,0-.09L19,5.4a6,6,0,0,1,8.91,6.21ZM11.08,17.15,8.38,15.6a.14.14,0,0,1-.05-.08V8.1a6,6,0,0,1,9.84-4.61L18,3.6,11.61,7.28a1,1,0,0,0-.53.91ZM12.54,14,16,12l3.47,2v4L16,20l-3.47-2Z"
                  fill="currentColor"></path>
              </svg>
            </span>
          </div>
          <div class="text-sm">
            <p class="text-xs text-left">2024/1/27 12:38:00</p>
            <div class="flex item-end mt-2 flex-row gap-1">
              <div class="text-black bg-system min-w px-3 py-2 rounded-md">
                <div class="mkdown-body">
                  <p>
                    flex-basis 是 CSS 中 Flexbox 布局模型的一个属性。它用于设置伸缩项目的初始主轴尺寸。可以指定一个固定的长度值，比如 flex-basis: 300px;，或者使用相对值，比如
                    flex-basis: 50%;。这个属性通常与 flex-grow 和 flex-shrink 属性一起使用来控制伸缩项目在 Flex 容器中的布局行为。
                  </p>
                </div>
              </div>
              <div class="flex flex-col">
                <button class="mb-2 transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-300">
                  <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M18.537 19.567A9.961 9.961 0 0 1 12 22C6.477 22 2 17.523 2 12S6.477 2 12 2s10 4.477 10 10c0 2.136-.67 4.116-1.81 5.74L17 12h3a8 8 0 1 0-2.46 5.772z">
                    </path>
                  </svg></button><button class="transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-200">
                    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M12 3c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0 14c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0-7c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2">
                    </path>
                  </svg>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="flex mb-6 flex-row-reverse">
          <div class="item-content ml-2 basis-8 flex items-center flex-shrink-0 h-8 justify-center">
            <span class="text-icon">
              <img src="/public/user.jpg" width="34px">
            </span>
          </div>
          <div class="text-sm">
            <p class="text-xs text-right">2024/1/27 12:38:00</p>
            <div class="flex item-end mt-2 flex-row-reverse gap-1">
              <div class="text-black bg-user min-w px-3 py-2 rounded-md">
                <div class="mkdown-body">
                  <p>
                    flex-basis 是 CSS 中 Flexbox 布局模型的一个属性。它用于设置伸缩项目的初始主轴尺寸。可以指定一个固定的长度值?
                  </p>
                </div>
              </div>
              <div class="flex flex-col">
                <button class="transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-200">
                    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M12 3c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0 14c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0-7c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2">
                    </path>
                  </svg>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="flex mb-6 flex-row">
          <div class="item-content mr-2 basis-8 flex items-center flex-shrink-0 h-8 justify-center">
            <span class="text-icon">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32" aria-hidden="true" width="1em" height="1em">
                <path
                  d="M29.71,13.09A8.09,8.09,0,0,0,20.34,2.68a8.08,8.08,0,0,0-13.7,2.9A8.08,8.08,0,0,0,2.3,18.9,8,8,0,0,0,3,25.45a8.08,8.08,0,0,0,8.69,3.87,8,8,0,0,0,6,2.68,8.09,8.09,0,0,0,7.7-5.61,8,8,0,0,0,5.33-3.86A8.09,8.09,0,0,0,29.71,13.09Zm-12,16.82a6,6,0,0,1-3.84-1.39l.19-.11,6.37-3.68a1,1,0,0,0,.53-.91v-9l2.69,1.56a.08.08,0,0,1,.05.07v7.44A6,6,0,0,1,17.68,29.91ZM4.8,24.41a6,6,0,0,1-.71-4l.19.11,6.37,3.68a1,1,0,0,0,1,0l7.79-4.49V22.8a.09.09,0,0,1,0,.08L13,26.6A6,6,0,0,1,4.8,24.41ZM3.12,10.53A6,6,0,0,1,6.28,7.9v7.57a1,1,0,0,0,.51.9l7.75,4.47L11.85,22.4a.14.14,0,0,1-.09,0L5.32,18.68a6,6,0,0,1-2.2-8.18Zm22.13,5.14-7.78-4.52L20.16,9.6a.08.08,0,0,1,.09,0l6.44,3.72a6,6,0,0,1-.9,10.81V16.56A1.06,1.06,0,0,0,25.25,15.67Zm2.68-4-.19-.12-6.36-3.7a1,1,0,0,0-1.05,0l-7.78,4.49V9.2a.09.09,0,0,1,0-.09L19,5.4a6,6,0,0,1,8.91,6.21ZM11.08,17.15,8.38,15.6a.14.14,0,0,1-.05-.08V8.1a6,6,0,0,1,9.84-4.61L18,3.6,11.61,7.28a1,1,0,0,0-.53.91ZM12.54,14,16,12l3.47,2v4L16,20l-3.47-2Z"
                  fill="currentColor"></path>
              </svg>
            </span>
          </div>
          <div class="text-sm">
            <p class="text-xs text-left">2024/1/27 12:38:00</p>
            <div class="flex item-end mt-2 flex-row gap-1">
              <div class="text-black bg-system min-w px-3 py-2 rounded-md">
                <div class="mkdown-body">
                  <p>
                    flex-basis 是 CSS 中 Flexbox 布局模型的一个属性。它用于设置伸缩项目的初始主轴尺寸。可以指定一个固定的长度值，比如 flex-basis: 300px;，或者使用相对值，比如
                    flex-basis: 50%;。这个属性通常与 flex-grow 和 flex-shrink 属性一起使用来控制伸缩项目在 Flex 容器中的布局行为。
                  </p>
                </div>
              </div>
              <div class="flex flex-col">
                <button class="mb-2 transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-300">
                  <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M18.537 19.567A9.961 9.961 0 0 1 12 22C6.477 22 2 17.523 2 12S6.477 2 12 2s10 4.477 10 10c0 2.136-.67 4.116-1.81 5.74L17 12h3a8 8 0 1 0-2.46 5.772z">
                    </path>
                  </svg></button><button class="transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-200">
                    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M12 3c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0 14c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0-7c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2">
                    </path>
                  </svg>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="flex mb-6 flex-row-reverse">
          <div class="item-content ml-2 basis-8 flex items-center flex-shrink-0 h-8 justify-center">
            <span class="text-icon">
              <img src="/public/user.jpg" width="34px">
            </span>
          </div>
          <div class="text-sm">
            <p class="text-xs text-right">2024/1/27 12:38:00</p>
            <div class="flex item-end mt-2 flex-row-reverse gap-1">
              <div class="text-black bg-user min-w px-3 py-2 rounded-md">
                <div class="mkdown-body">
                  <p>
                    flex-basis 是 CSS 中 Flexbox 布局模型的一个属性。它用于设置伸缩项目的初始主轴尺寸。可以指定一个固定的长度值?
                  </p>
                </div>
              </div>
              <div class="flex flex-col">
                <button class="transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-200">
                    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M12 3c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0 14c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0-7c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2">
                    </path>
                  </svg>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="flex mb-6 flex-row">
          <div class="item-content mr-2 basis-8 flex items-center flex-shrink-0 h-8 justify-center">
            <span class="text-icon">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32" aria-hidden="true" width="1em" height="1em">
                <path
                  d="M29.71,13.09A8.09,8.09,0,0,0,20.34,2.68a8.08,8.08,0,0,0-13.7,2.9A8.08,8.08,0,0,0,2.3,18.9,8,8,0,0,0,3,25.45a8.08,8.08,0,0,0,8.69,3.87,8,8,0,0,0,6,2.68,8.09,8.09,0,0,0,7.7-5.61,8,8,0,0,0,5.33-3.86A8.09,8.09,0,0,0,29.71,13.09Zm-12,16.82a6,6,0,0,1-3.84-1.39l.19-.11,6.37-3.68a1,1,0,0,0,.53-.91v-9l2.69,1.56a.08.08,0,0,1,.05.07v7.44A6,6,0,0,1,17.68,29.91ZM4.8,24.41a6,6,0,0,1-.71-4l.19.11,6.37,3.68a1,1,0,0,0,1,0l7.79-4.49V22.8a.09.09,0,0,1,0,.08L13,26.6A6,6,0,0,1,4.8,24.41ZM3.12,10.53A6,6,0,0,1,6.28,7.9v7.57a1,1,0,0,0,.51.9l7.75,4.47L11.85,22.4a.14.14,0,0,1-.09,0L5.32,18.68a6,6,0,0,1-2.2-8.18Zm22.13,5.14-7.78-4.52L20.16,9.6a.08.08,0,0,1,.09,0l6.44,3.72a6,6,0,0,1-.9,10.81V16.56A1.06,1.06,0,0,0,25.25,15.67Zm2.68-4-.19-.12-6.36-3.7a1,1,0,0,0-1.05,0l-7.78,4.49V9.2a.09.09,0,0,1,0-.09L19,5.4a6,6,0,0,1,8.91,6.21ZM11.08,17.15,8.38,15.6a.14.14,0,0,1-.05-.08V8.1a6,6,0,0,1,9.84-4.61L18,3.6,11.61,7.28a1,1,0,0,0-.53.91ZM12.54,14,16,12l3.47,2v4L16,20l-3.47-2Z"
                  fill="currentColor"></path>
              </svg>
            </span>
          </div>
          <div class="text-sm">
            <p class="text-xs text-left">2024/1/27 12:38:00</p>
            <div class="flex item-end mt-2 flex-row gap-1">
              <div class="text-black bg-system min-w px-3 py-2 rounded-md">
                <div class="mkdown-body">
                  <p>
                    flex-basis 是 CSS 中 Flexbox 布局模型的一个属性。它用于设置伸缩项目的初始主轴尺寸。可以指定一个固定的长度值，比如 flex-basis: 300px;，或者使用相对值，比如
                    flex-basis: 50%;。这个属性通常与 flex-grow 和 flex-shrink 属性一起使用来控制伸缩项目在 Flex 容器中的布局行为。
                  </p>
                </div>
              </div>
              <div class="flex flex-col">
                <button class="mb-2 transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-300">
                  <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M18.537 19.567A9.961 9.961 0 0 1 12 22C6.477 22 2 17.523 2 12S6.477 2 12 2s10 4.477 10 10c0 2.136-.67 4.116-1.81 5.74L17 12h3a8 8 0 1 0-2.46 5.772z">
                    </path>
                  </svg></button><button class="transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-200">
                    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M12 3c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0 14c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0-7c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2">
                    </path>
                  </svg>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="flex mb-6 flex-row-reverse">
          <div class="item-content ml-2 basis-8 flex items-center flex-shrink-0 h-8 justify-center">
            <span class="text-icon">
              <img src="/public/user.jpg" width="34px">
            </span>
          </div>
          <div class="text-sm">
            <p class="text-xs text-right">2024/1/27 12:38:00</p>
            <div class="flex item-end mt-2 flex-row-reverse gap-1">
              <div class="text-black bg-user min-w px-3 py-2 rounded-md">
                <div class="mkdown-body">
                  <p>
                    flex-basis 是 CSS 中 Flexbox 布局模型的一个属性。它用于设置伸缩项目的初始主轴尺寸。可以指定一个固定的长度值?
                  </p>
                </div>
              </div>
              <div class="flex flex-col">
                <button class="transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-200">
                    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M12 3c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0 14c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0-7c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2">
                    </path>
                  </svg>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="flex mb-6 flex-row">
          <div class="item-content mr-2 basis-8 flex items-center flex-shrink-0 h-8 justify-center">
            <span class="text-icon">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32" aria-hidden="true" width="1em" height="1em">
                <path
                  d="M29.71,13.09A8.09,8.09,0,0,0,20.34,2.68a8.08,8.08,0,0,0-13.7,2.9A8.08,8.08,0,0,0,2.3,18.9,8,8,0,0,0,3,25.45a8.08,8.08,0,0,0,8.69,3.87,8,8,0,0,0,6,2.68,8.09,8.09,0,0,0,7.7-5.61,8,8,0,0,0,5.33-3.86A8.09,8.09,0,0,0,29.71,13.09Zm-12,16.82a6,6,0,0,1-3.84-1.39l.19-.11,6.37-3.68a1,1,0,0,0,.53-.91v-9l2.69,1.56a.08.08,0,0,1,.05.07v7.44A6,6,0,0,1,17.68,29.91ZM4.8,24.41a6,6,0,0,1-.71-4l.19.11,6.37,3.68a1,1,0,0,0,1,0l7.79-4.49V22.8a.09.09,0,0,1,0,.08L13,26.6A6,6,0,0,1,4.8,24.41ZM3.12,10.53A6,6,0,0,1,6.28,7.9v7.57a1,1,0,0,0,.51.9l7.75,4.47L11.85,22.4a.14.14,0,0,1-.09,0L5.32,18.68a6,6,0,0,1-2.2-8.18Zm22.13,5.14-7.78-4.52L20.16,9.6a.08.08,0,0,1,.09,0l6.44,3.72a6,6,0,0,1-.9,10.81V16.56A1.06,1.06,0,0,0,25.25,15.67Zm2.68-4-.19-.12-6.36-3.7a1,1,0,0,0-1.05,0l-7.78,4.49V9.2a.09.09,0,0,1,0-.09L19,5.4a6,6,0,0,1,8.91,6.21ZM11.08,17.15,8.38,15.6a.14.14,0,0,1-.05-.08V8.1a6,6,0,0,1,9.84-4.61L18,3.6,11.61,7.28a1,1,0,0,0-.53.91ZM12.54,14,16,12l3.47,2v4L16,20l-3.47-2Z"
                  fill="currentColor"></path>
              </svg>
            </span>
          </div>
          <div class="text-sm">
            <p class="text-xs text-left">2024/1/27 12:38:00</p>
            <div class="flex item-end mt-2 flex-row gap-1">
              <div class="text-black bg-system min-w px-3 py-2 rounded-md">
                <div class="mkdown-body">
                  <p>
                    flex-basis 是 CSS 中 Flexbox 布局模型的一个属性。它用于设置伸缩项目的初始主轴尺寸。可以指定一个固定的长度值，比如 flex-basis: 300px;，或者使用相对值，比如
                    flex-basis: 50%;。这个属性通常与 flex-grow 和 flex-shrink 属性一起使用来控制伸缩项目在 Flex 容器中的布局行为。
                  </p>
                </div>
              </div>
              <div class="flex flex-col">
                <button class="mb-2 transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-300">
                  <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M18.537 19.567A9.961 9.961 0 0 1 12 22C6.477 22 2 17.523 2 12S6.477 2 12 2s10 4.477 10 10c0 2.136-.67 4.116-1.81 5.74L17 12h3a8 8 0 1 0-2.46 5.772z">
                    </path>
                  </svg></button><button class="transition text-neutral-300 hover:text-neutral-800 dark:hover:text-neutral-200">
                    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                    role="img" class=" iconify iconify--ri" width="1em" height="1em" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M12 3c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0 14c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2m0-7c-1.1 0-2 .9-2 2s.9 2 2 2s2-.9 2-2s-.9-2-2-2">
                    </path>
                  </svg>
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>
<style>
div {
  display: block;
}

.item-content {
  justify-content: center;
  align-items: center;
  border-radius: 999px;
  overflow: hidden;
}

.h-8 {
  height: 3rem;
}

.flex-shrink-0,
.shrink-0 {
  flex-shrink: 0;
}

.overflow-hidden {
  overflow: hidden;
}

.justify-center {
  justify-content: center;
}

.items-center {
  align-items: center;
}

.text-right {
  text-align: right;
}

.text-left {
  text-align: left;
}

.bg-user {
  --tw-bg-opacity: 1;
  background-color: rgb(210 249 209 / var(--tw-bg-opacity));
}

.bg-system {
  --tw-bg-opacity: 1;
  background-color: rgb(244 246 248 / var(--tw-bg-opacity));
}

.mkdown-body {
  background-color: transparent;
  font-size: 14px;
  font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Noto Sans, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji";
  margin: 0;
  line-height: 1.5;
}

.basis-8 {
  flex-basis: 2rem;
}

.flex {
  display: flex;
}

.text-icon {
  font-size: 28px;
}

p {
  display: block;
  white-space: pre-wrap;
  margin-block-start: 0em;
  margin-block-end: 0em;
  margin-inline-start: 0px;
  margin-inline-end: 0px;
}

.py-2 {
  padding-top: 0.5rem;
  padding-bottom: 0.5rem;
}

.px-3 {
  padding-left: 0.75rem;
  padding-right: 0.75rem;
}

.rounded-md {
  border-radius: 0.375rem;
}

.text-black {
  --tw-text-opacity: 1;
  color: rgb(0 0 0 / var(--tw-text-opacity));
}

.item-end {
  align-items: flex-end;
}



.text-xs {
  font-size: .75rem;
  line-height: 1rem;
  --tw-text-opacity: 1;
  color: rgb(180 187 196 / var(--tw-text-opacity));
  margin: 0;
}

.min-w {
  min-width: 20px;
}

.ml-2 {
  margin-left: 0.5rem;
}

.mr-2 {
  margin-right: 0.5rem;
}

.left-main {
  z-index: 2;
  width: 100%;
  height: 100%;
  /* background-color: red; */
  overflow: hidden;
}

.main-layout {
  margin: auto;
  height: calc(100% - 126px);
  max-width: 1280px;
  overflow-y: auto;
  padding: 16px;
  overflow: hidden;
  /* background-color: blue; */
}

.mb-6 {
  display: flex;

  margin-bottom: 1.5rem;
}

.gap-1 {
  gap: 0.25rem;
}

.flex-row-reverse {
  flex-direction: row-reverse;
}

.flex-row {
  flex-direction: row;
}

.flex-col {
  flex-direction: column;
}

.text-neutral-300 {
  --tw-text-opacity: 1;
  color: rgb(212 212 212 / var(--tw-text-opacity));
}

.mb-2 {
  margin-bottom: 0.5rem;
}

.mt-2 {
  margin-top: 0.5rem;
}

button,
[role=button] {
  cursor: pointer;
  -webkit-appearance: button;
  background-color: transparent;
  background-image: none;
  padding: 0;
  border: 0;
  font-size: 100%;
}

svg {
  display: block;
}</style>
