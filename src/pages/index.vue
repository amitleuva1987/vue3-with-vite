<template>
  <div class="bg-white">
    <main>
      <!-- Hero section -->
      <div class="pb-8 sm:pb-12 lg:pb-12">
        <div class="overflow-hidden pt-8 sm:pt-12 lg:relative lg:py-48">
          <div class="mx-auto max-w-md px-4 sm:max-w-3xl sm:px-6 lg:grid lg:max-w-7xl lg:grid-cols-2 lg:gap-24 lg:px-8">
            <div>
              <div class="mt-20">
                <div>
                  <a href="#" class="inline-flex space-x-4">
                    <span class="rounded bg-indigo-50 px-2.5 py-1 text-sm font-semibold text-indigo-600">What's
                      new</span>
                    <span class="inline-flex items-center space-x-1 text-sm font-medium text-indigo-600">
                      <span>Latest updates..</span>
                      <ChevronRightIcon class="h-5 w-5" aria-hidden="true" />
                    </span>
                  </a>
                </div>
                <div class="mt-6 sm:max-w-xl">
                  <h2 class="text-4xl font-bold tracking-tight text-gray-900 sm:text-5xl">Uncover Your Competitors Advertising Strategy</h2>
                  <p class="mt-6 text-xl text-gray-500">Make better marketing decisions by learning what ads are already
                    successful. Get comprehensive data on profitable native campaigns.</p>
                </div>
                <form action="https://rudybekker.com/tag/discover360/" class="mt-12 sm:flex sm:w-full sm:max-w-lg">
                  <div class="min-w-0 flex-1">
                    <label for="hero-email" class="sr-only">Email address</label>
                    <input id="hero-email" type="email"
                      class="block w-full rounded-md border border-gray-300 px-5 py-3 text-base text-gray-900 placeholder-gray-500 shadow-sm focus:border-indigo-500 focus:ring-indigo-500"
                      placeholder="Enter your email" />
                  </div>
                  <div class="mt-4 sm:mt-0 sm:ml-3">
                    <button type="submit"
                      class="block w-full rounded-md border border-transparent bg-indigo-600 px-5 py-3 text-base font-medium text-white shadow hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:ring-offset-2 sm:px-10">Create
                      Account</button>
                  </div>
                </form>
                <div class="mt-6">
                  <div class="inline-flex items-center divide-x divide-gray-300">
                    <div class="flex flex-shrink-0 pr-5">
                      <StarIcon class="h-5 w-5 text-yellow-400" aria-hidden="true" />
                      <StarIcon class="h-5 w-5 text-yellow-400" aria-hidden="true" />
                      <StarIcon class="h-5 w-5 text-yellow-400" aria-hidden="true" />
                      <StarIcon class="h-5 w-5 text-yellow-400" aria-hidden="true" />
                      <StarIcon class="h-5 w-5 text-yellow-400" aria-hidden="true" />
                    </div>
                    <div class="min-w-0 flex-1 py-1 pl-5 text-sm text-gray-500 sm:py-3"><span
                        class="font-medium text-gray-900">Rated 5 stars</span> by over <span
                        class="font-medium text-indigo-600">500+ beta users</span></div>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div class="sm:mx-auto sm:max-w-3xl sm:px-6">
            <div class="py-12 sm:relative sm:mt-12 sm:py-16 lg:absolute lg:inset-y-0 lg:right-0 lg:w-1/2">
              <div class="hidden sm:block">
                <div
                  class="absolute inset-y-0 left-1/2 w-screen rounded-l-3xl bg-gray-50 lg:left-80 lg:right-0 lg:w-full" />
                <svg class="absolute top-8 right-1/2 -mr-3 lg:left-0 lg:m-0" width="404" height="392" fill="none"
                  viewBox="0 0 404 392">
                  <defs>
                    <pattern id="837c3e70-6c3a-44e6-8854-cc48c737b659" x="0" y="0" width="20" height="20"
                      patternUnits="userSpaceOnUse">
                      <rect x="0" y="0" width="4" height="4" class="text-gray-200" fill="currentColor" />
                    </pattern>
                  </defs>
                  <rect width="404" height="392" fill="url(#837c3e70-6c3a-44e6-8854-cc48c737b659)" />
                </svg>
              </div>
              <div class="relative -mr-40 pl-4 sm:mx-auto sm:max-w-3xl sm:px-0 lg:h-full lg:max-w-none lg:pl-12">
                <img
                  class="w-full rounded-md shadow-xl ring-1 ring-black ring-opacity-5 lg:h-full lg:w-auto lg:max-w-none"
                  src="/src/asset/img/d360-1.png" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div>
      <!-- Stats -->
      <stats />

      <!-- Alternating Feature Sections -->
      <div class="relative overflow-hidden pt-16 pb-32">
        <div aria-hidden="true" class="absolute inset-x-0 top-0 h-48 bg-white" />
        <div class="relative">
          <div class="lg:mx-auto lg:grid lg:max-w-7xl lg:grid-flow-col-dense lg:grid-cols-2 lg:gap-24 lg:px-8">
            <div class="mx-auto max-w-xl px-4 sm:px-6 lg:mx-0 lg:max-w-none lg:py-16 lg:px-0">
              <div>
                <div>
                  <span
                    class="flex h-12 w-12 items-center justify-center rounded-md bg-gradient-to-r from-purple-600 to-indigo-600">
                    <InboxIcon class="h-6 w-6 text-white" aria-hidden="true" />
                  </span>
                </div>
                <div class="mt-6">
                  <h2 class="text-3xl font-bold tracking-tight text-gray-900">Instantly find winning campaigns</h2>
                  <p class="mt-4 text-lg text-gray-500">Analyze <b>Billions</b> of successful campaigns from all major native
                    traffic sources</p>
                  <div class="mt-6">
                    <a href="https://dash.discover360.app/register"
                      class="inline-flex rounded-md border border-transparent bg-gradient-to-r from-purple-600 to-indigo-600 bg-origin-border px-4 py-2 text-base font-medium text-white shadow-sm hover:from-purple-700 hover:to-indigo-700">Get
                      started</a>
                  </div>
                </div>
              </div>
              <div class="mt-8 border-t border-gray-200 pt-6">
                <blockquote>
                  <div>
                    <p class="text-base text-gray-500">&ldquo;Absolute game changer. No more guessing or wasting
                      thousands on seeing what ads work and not&rdquo;</p>
                  </div>
                  <footer class="mt-3">
                    <div class="flex items-center space-x-3">
                      <div class="flex-shrink-0">
                        <img class="h-6 w-6 rounded-full"
                          src="https://images.unsplash.com/photo-1509783236416-c9ad59bae472?ixlib=rb-=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=8&w=1024&h=1024&q=80"
                          alt="" />
                      </div>
                      <div class="text-base font-medium text-gray-700">Marcia Hill, Digital Marketing Manager</div>
                    </div>
                  </footer>
                </blockquote>
              </div>
            </div>
            <div class="mt-12 sm:mt-16 lg:mt-0">
              <div class="-mr-48 pl-4 sm:pl-6 md:-mr-16 lg:relative lg:m-0 lg:h-full lg:px-0">
                <img
                  class="w-full rounded-xl shadow-xl ring-1 ring-black ring-opacity-5 lg:absolute lg:left-0 lg:h-full lg:w-auto lg:max-w-none"
                  src="/src/asset/img/d360-8.png" alt="Inbox user interface" />
              </div>
            </div>
          </div>
        </div>
        <div class="mt-24">
          <div class="lg:mx-auto lg:grid lg:max-w-7xl lg:grid-flow-col-dense lg:grid-cols-2 lg:gap-24 lg:px-8">
            <div class="mx-auto max-w-xl px-4 sm:px-6 lg:col-start-2 lg:mx-0 lg:max-w-none lg:py-32 lg:px-0">
              <div>
                <div>
                  <span
                    class="flex h-12 w-12 items-center justify-center rounded-md bg-gradient-to-r from-purple-600 to-indigo-600">
                    <SparklesIcon class="h-6 w-6 text-white" aria-hidden="true" />
                  </span>
                </div>
                <div class="mt-6">
                  <h2 class="text-3xl font-bold tracking-tight text-gray-900">Competitor Breakdown</h2>
                  <p class="mt-4 text-lg text-gray-500">Discover360 will show you ANY competitors running ads along with
                    the techonolgy they are using, insights into their campaigns preformance & targeting specifications
                    in 1 dashboard so you can see what works and replicate.</p>
                  <div class="mt-6">
                    <a href="https://dash.discover360.app/register"
                      class="inline-flex rounded-md border border-transparent bg-gradient-to-r from-purple-600 to-indigo-600 bg-origin-border px-4 py-2 text-base font-medium text-white shadow-sm hover:from-purple-700 hover:to-indigo-700">Get
                      started</a>
                  </div>
                </div>
              </div>
            </div>
            <div class="mt-12 sm:mt-16 lg:col-start-1 lg:mt-0">
              <div class="-ml-48 pr-4 sm:pr-6 md:-ml-16 lg:relative lg:m-0 lg:h-full lg:px-0">
                <img
                  class="w-full rounded-xl shadow-xl ring-1 ring-black ring-opacity-5 lg:absolute lg:right-0 lg:h-full lg:w-auto lg:max-w-none"
                  src="/src/asset/img/d360-4.png" alt="Customer profile user interface" />
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Gradient Feature Section -->
      <div class="bg-gradient-to-r from-purple-800 to-indigo-700">
        <div class="mx-auto max-w-4xl px-4 py-16 sm:px-6 sm:pt-20 sm:pb-24 lg:max-w-7xl lg:px-8 lg:pt-24">
          <h2 class="text-3xl font-bold tracking-tight text-white">DISCOVER360 FEATURES</h2>
          <p class="mt-4 max-w-3xl text-lg text-purple-200">Here is how Discover360 is going to have you making bank as
            early as today</p>
          <div
            class="mt-12 grid grid-cols-1 gap-x-6 gap-y-12 sm:grid-cols-2 lg:mt-16 lg:grid-cols-4 lg:gap-x-8 lg:gap-y-16">
            <div v-for="feature in features" :key="feature.name">
              <div>
                <span class="flex h-12 w-12 items-center justify-center rounded-md bg-white bg-opacity-10">
                  <component :is="feature.icon" class="h-6 w-6 text-white" aria-hidden="true" />
                </span>
              </div>
              <div class="mt-6">
                <h3 class="text-lg font-medium text-white">{{ feature.name }}</h3>
                <p class="mt-2 text-base text-purple-200">{{ feature.description }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </main>
  </div>
  <PricingBasic />
</template>

<script setup>
import { ChevronRightIcon, StarIcon } from '@heroicons/vue/20/solid'
import { defineComponent, h } from 'vue'
import { Popover, PopoverButton, PopoverGroup, PopoverPanel } from '@headlessui/vue'
import {
  ArrowUturnLeftIcon,
  Bars3Icon,
  ChatBubbleBottomCenterTextIcon,
  ChatBubbleLeftEllipsisIcon,
  ChatBubbleLeftRightIcon,
  DocumentChartBarIcon,
  HeartIcon,
  InboxIcon,
  PencilSquareIcon,
  QuestionMarkCircleIcon,
  SparklesIcon,
  TrashIcon,
  UsersIcon,
  XMarkIcon,
  BoltIcon,
} from '@heroicons/vue/24/outline'
import { ChevronDownIcon } from '@heroicons/vue/20/solid'

const features = [
  {
    name: 'Remove The Guesswork',
    description: 'Discover360 shows you exactly what ads are working NOW (and what are NOT) so you don’t waste money on ads that don’t work - Search for KEYWORDS, Niches, Competitors and even domains to see what ads are running & more importantly winning.',
    icon: BoltIcon,
  },
  {
    name: 'Generate Buyer Traffic Today With Ads',
    description: 'Remove the need to test, change, edit ads by allowing Discover360 to SHOW you the best performing ads in your niche.',
    icon: BoltIcon,
  },
  {
    name: 'Competitor Breakdown',
    description: 'Discover360 will show you ANY competitors running ads along with their landing page in 1 dashboard so you can see what works and replicate.',
    icon: BoltIcon,
  },
  {
    name: 'Worlds Largest Ad Database',
    description: 'Discover360 gives you the worlds largest fb ads library to search with over 80 million ads from 15 different countries with thousands of new ads added daily.',
    icon: BoltIcon,
  },
  {
    name: 'Demographic & Engagement Filters',
    description: 'These allow you to search ads based on gender, age, marital status & location along with searching most likes, comments or shares to see what users are engaging with the most.',
    icon: BoltIcon,
  },
  {
    name: 'Geo location filters',
    description: 'Hate not knowing which countries to target? Discover360 breaks down where any ad is being shown to allow you to better identify the audience you are targeting.',
    icon: BoltIcon,
  },
  {
    name: 'Video & Image Ad Integration',
    description: 'With video ads being a leading ad strategy, Discover360 will show you what video ads are working the best for YOUR niche in TODAYS market.',
    icon: BoltIcon,
  },
  {
    name: 'Technology Insights',
    description: 'Discover360 will not only show you the winning ADS , but also allow you to see the landing page the traffic is being sent to in 1 dashboard - allowing you to replicate the winning funnels.',
    icon: BoltIcon,
  },
]
</script>