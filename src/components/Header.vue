<template>
    <header>
      <Popover class="relative bg-white">
        <div class="mx-auto flex max-w-7xl items-center justify-between px-4 py-6 sm:px-6 md:justify-start md:space-x-10 lg:px-8">
          <div class="flex justify-start lg:w-0 lg:flex-1">
            <a href="/">
              <span class="sr-only">Discover360</span>
              <img class="h-8 w-auto sm:h-10" src="/src/asset/img/d360-white-new.svg" alt="" />
            </a>
          </div>
          <div class="-my-2 -mr-2 md:hidden">
            <PopoverButton class="inline-flex items-center justify-center rounded-md bg-white p-2 text-gray-400 hover:bg-gray-100 hover:text-gray-500 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500">
              <span class="sr-only">Open menu</span>
              <Bars3Icon class="h-6 w-6" aria-hidden="true" />
            </PopoverButton>
          </div>
          <PopoverGroup as="nav" class="hidden space-x-10 md:flex">
            <Popover class="relative" v-slot="{ open }">
              <PopoverButton :class="[open ? 'text-gray-900' : 'text-gray-500', 'group inline-flex items-center rounded-md bg-white text-base font-medium hover:text-gray-900 focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:ring-offset-2']">
                <span>Solutions</span>
                <ChevronDownIcon :class="[open ? 'text-gray-600' : 'text-gray-400', 'ml-2 h-5 w-5 group-hover:text-gray-500']" aria-hidden="true" />
              </PopoverButton>

              <transition enter-active-class="transition ease-out duration-200" enter-from-class="opacity-0 translate-y-1" enter-to-class="opacity-100 translate-y-0" leave-active-class="transition ease-in duration-150" leave-from-class="opacity-100 translate-y-0" leave-to-class="opacity-0 translate-y-1">
                <PopoverPanel class="absolute z-10 -ml-4 mt-3 w-screen max-w-md transform lg:left-1/2 lg:ml-0 lg:max-w-2xl lg:-translate-x-1/2">
                  <div class="overflow-hidden rounded-lg shadow-lg ring-1 ring-black ring-opacity-5">
                    <div class="relative grid gap-6 bg-white px-5 py-6 sm:gap-8 sm:p-8 lg:grid-cols-2">
                      <a v-for="item in solutions" :key="item.name" :href="item.href" class="-m-3 flex items-start rounded-lg p-3 hover:bg-gray-50">
                        <div class="flex h-10 w-10 flex-shrink-0 items-center justify-center rounded-md bg-gradient-to-r from-purple-600 to-indigo-600 text-white sm:h-12 sm:w-12">
                          <component :is="item.icon" class="h-6 w-6" aria-hidden="true" />
                        </div>
                        <div class="ml-4">
                          <p class="text-base font-medium text-gray-900">{{ item.name }}</p>
                          <p class="mt-1 text-sm text-gray-500">{{ item.description }}</p>
                        </div>
                      </a>
                    </div>
                  </div>
                </PopoverPanel>
              </transition>
            </Popover>
            <a href="/About" class="text-base font-medium text-gray-500 hover:text-gray-900">About</a>
            <a href="/Resources" class="text-base font-medium text-gray-500 hover:text-gray-900">Resources</a>
            <a href="/Jobs" class="text-base font-medium text-gray-500 hover:text-gray-900">Jobs</a>
          </PopoverGroup>
          <div class="hidden items-center justify-end md:flex md:flex-1 lg:w-0">
            <a href="https://dash.discover360.app/login" class="whitespace-nowrap text-base font-medium text-gray-500 hover:text-gray-900">Sign in</a>
            <a href="https://dash.discover360.app/register" class="ml-8 inline-flex items-center justify-center whitespace-nowrap rounded-md border border-transparent bg-gradient-to-r from-purple-600 to-indigo-600 bg-origin-border px-4 py-2 text-base font-medium text-white shadow-sm hover:from-purple-700 hover:to-indigo-700">Sign up</a>
          </div>
        </div>

        <transition enter-active-class="duration-200 ease-out" enter-from-class="opacity-0 scale-95" enter-to-class="opacity-100 scale-100" leave-active-class="duration-100 ease-in" leave-from-class="opacity-100 scale-100" leave-to-class="opacity-0 scale-95">
          <PopoverPanel focus class="absolute inset-x-0 top-0 z-30 origin-top-right transform p-2 transition md:hidden">
            <div class="divide-y-2 divide-gray-50 rounded-lg bg-white shadow-lg ring-1 ring-black ring-opacity-5">
              <div class="px-5 pt-5 pb-6">
                <div class="flex items-center justify-between">
                  <div>
                    <img class="h-8 w-auto" src="/src/asset/img/d360-white-new.svg" alt="Discover360" />
                  </div>
                  <div class="-mr-2">
                    <PopoverButton class="inline-flex items-center justify-center rounded-md bg-white p-2 text-gray-400 hover:bg-gray-100 hover:text-gray-500 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500">
                      <span class="sr-only">Close menu</span>
                      <XMarkIcon class="h-6 w-6" aria-hidden="true" />
                    </PopoverButton>
                  </div>
                </div>
                <div class="mt-6">
                  <nav class="grid grid-cols-1 gap-7">
                    <a v-for="item in solutions" :key="item.name" :href="item.href" class="-m-3 flex items-center rounded-lg p-3 hover:bg-gray-50">
                      <div class="flex h-10 w-10 flex-shrink-0 items-center justify-center rounded-md bg-gradient-to-r from-purple-600 to-indigo-600 text-white">
                        <component :is="item.icon" class="h-6 w-6" aria-hidden="true" />
                      </div>
                      <div class="ml-4 text-base font-medium text-gray-900">{{ item.name }}</div>
                    </a>
                  </nav>
                </div>
              </div>
              <div class="py-6 px-5">
                <div class="grid grid-cols-2 gap-4">
                  <a href="/Pricing" class="text-base font-medium text-gray-900 hover:text-gray-700">Pricing</a>
                  <a href="/About" class="text-base font-medium text-gray-900 hover:text-gray-700">About</a>
                  <a href="/Resources" class="text-base font-medium text-gray-900 hover:text-gray-700">Resources</a>
                  <a href="/Jobs" class="text-base font-medium text-gray-900 hover:text-gray-700">Jobs</a>
                </div>
                <div class="mt-6">
                  <a href="https://dash.discover360.app/register" class="flex w-full items-center justify-center rounded-md border border-transparent bg-gradient-to-r from-purple-600 to-indigo-600 bg-origin-border px-4 py-2 text-base font-medium text-white shadow-sm hover:from-purple-700 hover:to-indigo-700">Sign up</a>
                  <p class="mt-6 text-center text-base font-medium text-gray-500">
                    Existing customer?
                    <a href="https://dash.discover360.app/login" class="text-gray-900">Sign in</a>
                  </p>
                </div>
              </div>
            </div>
          </PopoverPanel>
        </transition>
      </Popover>
    </header>
</template>

<script setup>
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
} from '@heroicons/vue/24/outline'
import { ChevronDownIcon, BoltIcon } from '@heroicons/vue/20/solid'

const solutions = [
  {
    name: 'Instantly find winning campaigns',
    description: 'Analyze Billions of successful campaigns from all major native traffic sources',
    href: '/',
    icon: BoltIcon,
  },
  {
    name: 'White-Label SaaS Solution',
    description: 'Easily rebrand & resell Discover360 to your customers with our turnkey white-label SaaS solution.',
    href: '/SaaS',
    icon: BoltIcon,
  },
  {
    name: 'Advanced Data Harvesting',
    description: "Harvest any FB Group, Page, Post or Ad and get instant data deep data insights .",
    href: '#',
    icon: BoltIcon,
  },
  {
    name: 'API & Big Data',
    description: "Integrate our data into your Data Science, Machine Learning & AI Flows",
    href: '#',
    icon: BoltIcon,
  },
  {
    name: 'Mastermind',
    description: "Join our private Mastermind Group and get access to our top experts",
    href: '#',
    icon: BoltIcon,
  },
  {
    name: 'Consulting',
    description: "Get access to our top experts for 1-on-1 consulting",
    href: '#',
    icon: BoltIcon,
  },
]
</script>