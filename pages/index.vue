<template>
  <div class="flex flex-wrap gap-4 p-4">
    <section class="flex gap-4">
      <button class="btn">Button</button>
      <button class="btn btn-neutral">Neutral</button>
      <button class="btn btn-primary">Primary</button>
      <button class="btn btn-secondary">Secondary</button>
      <button class="btn btn-accent">Accent</button>
      <button class="btn btn-ghost">Ghost</button>
      <button class="btn btn-link">Link</button>
    </section>
    <section>
      <!-- Open the modal using ID.showModal() method -->
      <button class="btn" onclick="my_modal_1.showModal()">open modal</button>
      <dialog id="my_modal_1" class="modal">
        <div class="modal-box">
          <h3 class="font-bold text-lg">Hello!</h3>
          <p class="py-4">Press ESC key or click the button below to close</p>
          <div class="modal-action">
            <form method="dialog">
              <!-- if there is a button in form, it will close the modal -->
              <button class="btn">Close</button>
            </form>
          </div>
        </div>
      </dialog>
    </section>
    <section class="flex items-center gap-5">
      <div>
        <label class="swap">
          <input type="checkbox" />
          <div class="swap-on">ON</div>
          <div class="swap-off">OFF</div>
        </label>
      </div>
      <div>
        <label class="swap swap-rotate">

          <!-- this hidden checkbox controls the state -->
          <input type="checkbox" />

          <!-- sun icon -->
          <svg class="swap-on fill-current w-10 h-10" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
            <path
              d="M5.64,17l-.71.71a1,1,0,0,0,0,1.41,1,1,0,0,0,1.41,0l.71-.71A1,1,0,0,0,5.64,17ZM5,12a1,1,0,0,0-1-1H3a1,1,0,0,0,0,2H4A1,1,0,0,0,5,12Zm7-7a1,1,0,0,0,1-1V3a1,1,0,0,0-2,0V4A1,1,0,0,0,12,5ZM5.64,7.05a1,1,0,0,0,.7.29,1,1,0,0,0,.71-.29,1,1,0,0,0,0-1.41l-.71-.71A1,1,0,0,0,4.93,6.34Zm12,.29a1,1,0,0,0,.7-.29l.71-.71a1,1,0,1,0-1.41-1.41L17,5.64a1,1,0,0,0,0,1.41A1,1,0,0,0,17.66,7.34ZM21,11H20a1,1,0,0,0,0,2h1a1,1,0,0,0,0-2Zm-9,8a1,1,0,0,0-1,1v1a1,1,0,0,0,2,0V20A1,1,0,0,0,12,19ZM18.36,17A1,1,0,0,0,17,18.36l.71.71a1,1,0,0,0,1.41,0,1,1,0,0,0,0-1.41ZM12,6.5A5.5,5.5,0,1,0,17.5,12,5.51,5.51,0,0,0,12,6.5Zm0,9A3.5,3.5,0,1,1,15.5,12,3.5,3.5,0,0,1,12,15.5Z" />
          </svg>

          <!-- moon icon -->
          <svg class="swap-off fill-current w-10 h-10" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
            <path
              d="M21.64,13a1,1,0,0,0-1.05-.14,8.05,8.05,0,0,1-3.37.73A8.15,8.15,0,0,1,9.08,5.49a8.59,8.59,0,0,1,.25-2A1,1,0,0,0,8,2.36,10.14,10.14,0,1,0,22,14.05,1,1,0,0,0,21.64,13Zm-9.5,6.69A8.14,8.14,0,0,1,7.08,5.22v.27A10.15,10.15,0,0,0,17.22,15.63a9.79,9.79,0,0,0,2.1-.22A8.11,8.11,0,0,1,12.14,19.73Z" />
          </svg>

        </label>
      </div>
    </section>
    <section class="flex flex-wrap gap-4 p-4">
      <div class="collapse bg-base-200">
        <input type="radio" name="my-accordion-1" checked="checked" />
        <div class="collapse-title text-xl font-medium">
          Click to open this one and close others
        </div>
        <div class="collapse-content">
          <p>hello</p>
        </div>
      </div>
      <div class="collapse bg-base-200">
        <input type="radio" name="my-accordion-1" />
        <div class="collapse-title text-xl font-medium">
          Click to open this one and close others
        </div>
        <div class="collapse-content">
          <p>hello</p>
        </div>
      </div>
      <div class="collapse bg-base-200">
        <input type="radio" name="my-accordion-1" />
        <div class="collapse-title text-xl font-medium">
          Click to open this one and close others
        </div>
        <div class="collapse-content">
          <p>hello</p>
        </div>
      </div>
    </section>
    <section class="p-4">
      <div class="avatar">
        <div class="w-24 rounded-xl">
          <img src="https://img.daisyui.com/images/stock/photo-1534528741775-53994a69daeb.jpg" />
        </div>
      </div>
      <div class="avatar ml-2">
        <div class="w-24 rounded-full">
          <img src="https://img.daisyui.com/images/stock/photo-1534528741775-53994a69daeb.jpg" />
        </div>
      </div>
    </section>
    <section>
      <div class="badge">default</div>
      <div class="badge badge-neutral">neutral</div>
      <div class="badge badge-primary">primary</div>
      <div class="badge badge-secondary">secondary</div>
      <div class="badge badge-accent">accent</div>
      <div class="badge badge-ghost">ghost</div>
    </section>
    <section>
      <div class="card w-96 bg-base-100 shadow-xl">
        <figure><img src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.jpg" alt="Shoes" />
        </figure>
        <div class="card-body">
          <h2 class="card-title">Shoes!</h2>
          <p>If a dog chews shoes whose shoes does he choose?</p>
          <div class="card-actions justify-end">
            <button class="btn btn-primary">Buy Now</button>
          </div>
        </div>
      </div>
    </section>
    <section class="border border-primary p-4 rounded">
      <div class="chat chat-start">
        <div class="chat-bubble chat-bubble-primary">What kind of nonsense is this</div>
      </div>
      <div class="chat chat-start">
        <div class="chat-bubble chat-bubble-secondary">Put me on the Council and not make me a Master!??</div>
      </div>
      <div class="chat chat-start">
        <div class="chat-bubble chat-bubble-accent">That's never been done in the history of the Jedi. It's insulting!
        </div>
      </div>
      <div class="chat chat-end">
        <div class="chat-bubble chat-bubble-info">Calm down, Anakin.</div>
      </div>
      <div class="chat chat-end">
        <div class="chat-bubble chat-bubble-success">You have been given a great honor.</div>
      </div>
      <div class="chat chat-end">
        <div class="chat-bubble chat-bubble-warning">To be on the Council at your age.</div>
      </div>
      <div class="chat chat-end">
        <div class="chat-bubble chat-bubble-error">It's never happened before.</div>
      </div>
    </section>
    <section class="flex flex-col gap-4 p-4 justify-center items-center">
      <div>
        <div class="grid grid-flow-col gap-5 text-center auto-cols-max">
          <div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
            <span class="countdown font-mono text-5xl">
              <span style="--value:15;"></span>
            </span>
            days
          </div>
          <div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
            <span class="countdown font-mono text-5xl">
              <span style="--value:10;"></span>
            </span>
            hours
          </div>
          <div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
            <span class="countdown font-mono text-5xl">
              <span style="--value:24;"></span>
            </span>
            min
          </div>
          <div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
            <span class="countdown font-mono text-5xl">
              <span style="--value:50;"></span>
            </span>
            sec
          </div>
        </div>
      </div>
      <div>
        <div class="grid grid-flow-col gap-5 text-center auto-cols-max">
          <div class="flex flex-col">
            <span class="countdown font-mono text-5xl">
              <span style="--value:15;"></span>
            </span>
            days
          </div>
          <div class="flex flex-col">
            <span class="countdown font-mono text-5xl">
              <span style="--value:10;"></span>
            </span>
            hours
          </div>
          <div class="flex flex-col">
            <span class="countdown font-mono text-5xl">
              <span style="--value:24;"></span>
            </span>
            min
          </div>
          <div class="flex flex-col">
            <span class="countdown font-mono text-5xl">
              <span style="--value:20;"></span>
            </span>
            sec
          </div>
        </div>
      </div>
      <div>
        <div class="flex gap-5">
          <div>
            <span class="countdown font-mono text-4xl">
              <span style="--value:15;"></span>
            </span>
            days
          </div>
          <div>
            <span class="countdown font-mono text-4xl">
              <span style="--value:10;"></span>
            </span>
            hours
          </div>
          <div>
            <span class="countdown font-mono text-4xl">
              <span style="--value:24;"></span>
            </span>
            min
          </div>
          <div>
            <span class="countdown font-mono text-4xl">
              <span style="--value:31;"></span>
            </span>
            sec
          </div>
        </div>
      </div>
    </section>
    <section>
      <div class="stats shadow">

        <div class="stat">
          <div class="stat-figure text-primary">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
              class="inline-block w-8 h-8 stroke-current">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z">
              </path>
            </svg>
          </div>
          <div class="stat-title">Total Likes</div>
          <div class="stat-value text-primary">25.6K</div>
          <div class="stat-desc">21% more than last month</div>
        </div>

        <div class="stat">
          <div class="stat-figure text-secondary">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
              class="inline-block w-8 h-8 stroke-current">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z">
              </path>
            </svg>
          </div>
          <div class="stat-title">Page Views</div>
          <div class="stat-value text-secondary">2.6M</div>
          <div class="stat-desc">21% more than last month</div>
        </div>

        <div class="stat">
          <div class="stat-figure text-secondary">
            <div class="avatar online">
              <div class="w-16 rounded-full">
                <img src="https://img.daisyui.com/images/stock/photo-1534528741775-53994a69daeb.jpg" />
              </div>
            </div>
          </div>
          <div class="stat-value">86%</div>
          <div class="stat-title">Tasks done</div>
          <div class="stat-desc text-secondary">31 tasks remaining</div>
        </div>
      </div>
    </section>
    <section>
      <ul class="steps">
        <li class="step step-primary">Register</li>
        <li class="step step-primary">Choose plan</li>
        <li class="step">Purchase</li>
        <li class="step">Receive Product</li>
      </ul>
    </section>
    <section>
      <span class="loading loading-spinner text-primary"></span>
      <span class="loading loading-spinner text-secondary"></span>
      <span class="loading loading-spinner text-accent"></span>
      <span class="loading loading-spinner text-neutral"></span>
      <span class="loading loading-spinner text-info"></span>
      <span class="loading loading-spinner text-success"></span>
      <span class="loading loading-spinner text-warning"></span>
      <span class="loading loading-spinner text-error"></span>
    </section>
    <section class="flex flex-col gap-4">
      <progress class="progress w-56"></progress>
      <progress class="progress progress-error w-56" value="0" max="100"></progress>
      <progress class="progress progress-error w-56" value="10" max="100"></progress>
      <progress class="progress progress-error w-56" value="40" max="100"></progress>
      <progress class="progress progress-error w-56" value="70" max="100"></progress>
      <progress class="progress progress-error w-56" value="100" max="100"></progress>
    </section>
    <section class="flex gap-3">
      <div class="radial-progress" style="--value:0;" role="progressbar">0%</div>
      <div class="radial-progress" style="--value:20;" role="progressbar">20%</div>
      <div class="radial-progress" style="--value:60;" role="progressbar">60%</div>
      <div class="radial-progress" style="--value:80;" role="progressbar">80%</div>
      <div class="radial-progress" style="--value:100;" role="progressbar">100%</div>
      <div class="radial-progress bg-primary text-primary-content border-4 border-primary" style="--value:70;"
        role="progressbar">70%</div>
    </section>
    <section>
      <div class="flex flex-col gap-4 w-52">
        <div class="skeleton h-32 w-full"></div>
        <div class="skeleton h-4 w-28"></div>
        <div class="skeleton h-4 w-full"></div>
        <div class="skeleton h-4 w-full"></div>
      </div>
    </section>
    <section class="flex flex-col gap-4 items-center">
      <input type="checkbox" checked="checked" class="checkbox checkbox-xs" />
      <input type="checkbox" checked="checked" class="checkbox checkbox-sm" />
      <input type="checkbox" checked="checked" class="checkbox checkbox-md" />
      <input type="checkbox" checked="checked" class="checkbox checkbox-lg" />
    </section>
    <section>
      <label class="form-control w-full max-w-xs">
        <div class="label">
          <span class="label-text">Pick a file</span>
          <span class="label-text-alt">Alt label</span>
        </div>
        <input type="file" class="file-input file-input-bordered w-full max-w-xs" />
        <div class="label">
          <span class="label-text-alt">Alt label</span>
          <span class="label-text-alt">Alt label</span>
        </div>
      </label>
    </section>
    <section>
      <input type="radio" name="radio-1" class="radio" checked />
      <input type="radio" name="radio-1" class="radio" />
    </section>
    <section>
      <input type="range" min="0" max="100" value="40" class="range" />
      <input type="range" min="0" max="100" value="25" class="range" step="25" />
      <div class="w-full flex justify-between text-xs px-2">
        <span>|</span>
        <span>|</span>
        <span>|</span>
        <span>|</span>
        <span>|</span>
      </div>
      <input type="range" min="0" max="100" value="40" class="range range-primary mt-2" />
    </section>
    <section class="flex flex-col gap-4 items-center">
      <!-- xs -->
      <div class="rating rating-xs">
        <input type="radio" name="rating-5" class="mask mask-star-2 bg-orange-400" />
        <input type="radio" name="rating-5" class="mask mask-star-2 bg-orange-400" checked />
        <input type="radio" name="rating-5" class="mask mask-star-2 bg-orange-400" />
        <input type="radio" name="rating-5" class="mask mask-star-2 bg-orange-400" />
        <input type="radio" name="rating-5" class="mask mask-star-2 bg-orange-400" />
      </div>
      <!-- sm -->
      <div class="rating rating-sm">
        <input type="radio" name="rating-6" class="mask mask-star-2 bg-orange-400" />
        <input type="radio" name="rating-6" class="mask mask-star-2 bg-orange-400" checked />
        <input type="radio" name="rating-6" class="mask mask-star-2 bg-orange-400" />
        <input type="radio" name="rating-6" class="mask mask-star-2 bg-orange-400" />
        <input type="radio" name="rating-6" class="mask mask-star-2 bg-orange-400" />
      </div>
      <!-- md -->
      <div class="rating rating-md">
        <input type="radio" name="rating-7" class="mask mask-star-2 bg-orange-400" />
        <input type="radio" name="rating-7" class="mask mask-star-2 bg-orange-400" checked />
        <input type="radio" name="rating-7" class="mask mask-star-2 bg-orange-400" />
        <input type="radio" name="rating-7" class="mask mask-star-2 bg-orange-400" />
        <input type="radio" name="rating-7" class="mask mask-star-2 bg-orange-400" />
      </div>
      <!-- lg -->
      <div class="rating rating-lg">
        <input type="radio" name="rating-8" class="mask mask-star-2 bg-orange-400" />
        <input type="radio" name="rating-8" class="mask mask-star-2 bg-orange-400" checked />
        <input type="radio" name="rating-8" class="mask mask-star-2 bg-orange-400" />
        <input type="radio" name="rating-8" class="mask mask-star-2 bg-orange-400" />
        <input type="radio" name="rating-8" class="mask mask-star-2 bg-orange-400" />
      </div>
    </section>
    <section class="flex flex-row gap-5">
      <div class="flex flex-col gap-2">
        <label class="input input-bordered flex items-center gap-2">
          <input type="text" class="grow" placeholder="Search" />
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor" class="w-4 h-4 opacity-70">
            <path fill-rule="evenodd"
              d="M9.965 11.026a5 5 0 1 1 1.06-1.06l2.755 2.754a.75.75 0 1 1-1.06 1.06l-2.755-2.754ZM10.5 7a3.5 3.5 0 1 1-7 0 3.5 3.5 0 0 1 7 0Z"
              clip-rule="evenodd" />
          </svg>
        </label>
        <label class="input input-bordered flex items-center gap-2">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor" class="w-4 h-4 opacity-70">
            <path
              d="M2.5 3A1.5 1.5 0 0 0 1 4.5v.793c.026.009.051.02.076.032L7.674 8.51c.206.1.446.1.652 0l6.598-3.185A.755.755 0 0 1 15 5.293V4.5A1.5 1.5 0 0 0 13.5 3h-11Z" />
            <path
              d="M15 6.954 8.978 9.86a2.25 2.25 0 0 1-1.956 0L1 6.954V11.5A1.5 1.5 0 0 0 2.5 13h11a1.5 1.5 0 0 0 1.5-1.5V6.954Z" />
          </svg>
          <input type="text" class="grow" placeholder="Email" />
        </label>
        <label class="input input-bordered flex items-center gap-2">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor" class="w-4 h-4 opacity-70">
            <path
              d="M8 8a3 3 0 1 0 0-6 3 3 0 0 0 0 6ZM12.735 14c.618 0 1.093-.561.872-1.139a6.002 6.002 0 0 0-11.215 0c-.22.578.254 1.139.872 1.139h9.47Z" />
          </svg>
          <input type="text" class="grow" placeholder="Username" />
        </label>
        <label class="input input-bordered flex items-center gap-2">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor" class="w-4 h-4 opacity-70">
            <path fill-rule="evenodd"
              d="M14 6a4 4 0 0 1-4.899 3.899l-1.955 1.955a.5.5 0 0 1-.353.146H5v1.5a.5.5 0 0 1-.5.5h-2a.5.5 0 0 1-.5-.5v-2.293a.5.5 0 0 1 .146-.353l3.955-3.955A4 4 0 1 1 14 6Zm-4-2a.75.75 0 0 0 0 1.5.5.5 0 0 1 .5.5.75.75 0 0 0 1.5 0 2 2 0 0 0-2-2Z"
              clip-rule="evenodd" />
          </svg>
          <input type="password" class="grow" value="password" />
        </label>
      </div>
      <div class="flex flex-col gap-2">
        <label class="input input-bordered flex items-center gap-2">
          Name
          <input type="text" class="grow" placeholder="Daisy" />
        </label>
        <label class="input input-bordered flex items-center gap-2">
          Email
          <input type="text" class="grow" placeholder="daisy@site.com" />
        </label>
        <label class="input input-bordered flex items-center gap-2">
          <input type="text" class="grow" placeholder="Search" />
          <kbd class="kbd kbd-sm">⌘</kbd>
          <kbd class="kbd kbd-sm">K</kbd>
        </label>
        <label class="input input-bordered flex items-center gap-2">
          <input type="text" class="grow" placeholder="Search" />
          <span class="badge badge-info">Optional</span>
        </label>
      </div>
      <div>
        <textarea class="textarea textarea-bordered" placeholder="Bio"></textarea>
      </div>
    </section>
    <section class="flex flex-col gap-3">
      <input type="checkbox" class="toggle toggle-success" checked />
      <input type="checkbox" class="toggle toggle-warning" checked />
      <input type="checkbox" class="toggle toggle-info" checked />
      <input type="checkbox" class="toggle toggle-error" checked />
    </section>
    <section class="flex flex-row gap-3">
      <div class="flex flex-col gap-3 w-[500px]">
        <div class="flex flex-col w-full">
          <div class="divider divider-start">Start</div>
          <div class="divider">Default</div>
          <div class="divider divider-end">End</div>
        </div>
      </div>
    </section>
    <section class="flex flex-wrap gap-4">
      <div class="indicator">
        <span class="indicator-item badge badge-secondary"></span>
        <div class="grid w-32 h-32 bg-base-300 place-items-center">content</div>
      </div>
      <div class="indicator">
        <span class="indicator-item badge badge-secondary">99+</span>
        <button class="btn">inbox</button>
      </div>
    </section>
    <section class="flex flex-col gap-3">
      <div class="join">
        <div>
          <div>
            <input class="input input-bordered join-item" placeholder="Search" />
          </div>
        </div>
        <select class="select select-bordered join-item">
          <option disabled selected>Filter</option>
          <option>Sci-fi</option>
          <option>Drama</option>
          <option>Action</option>
        </select>
        <div class="indicator">
          <span class="indicator-item badge badge-secondary">new</span>
          <button class="btn join-item">Search</button>
        </div>
      </div>
      <div class="join">
        <input class="input input-bordered join-item" placeholder="Email" />
        <button class="btn join-item rounded-r-full">Subscribe</button>
      </div>
    </section>
  </div>
</template>

<script lang="ts" setup>

</script>

<style></style>