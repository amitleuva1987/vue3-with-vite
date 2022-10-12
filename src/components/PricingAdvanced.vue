<template>
  <div class="bg-white">
    <div class="pt-12 sm:pt-16 lg:pt-24">
      <div class="mx-auto max-w-7xl px-4 text-center sm:px-6 lg:px-8">
        <div class="mx-auto max-w-3xl space-y-2 lg:max-w-none">
          <h2 class="block text-center text-lg font-semibold text-indigo-600">Pricing</h2>
          <p class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl lg:text-5xl">Exclusive WL SaaS Deal</p>
          <p class="text-xl text-gray-900">100 Licenses Available</p>
        </div>
      </div>
    </div>
    <div class="mt-8 bg-white pb-12 sm:mt-12 sm:pb-16 lg:mt-16 lg:pb-24">
      <div class="relative">
        <div class="absolute inset-0 h-3/4 bg-white" />
        <div class="relative z-10 mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
          <div class="mx-auto max-w-md space-y-4 lg:grid lg:max-w-5xl lg:grid-cols-2 lg:gap-5 lg:space-y-0">
            <div v-for="tier in tiers" :key="tier.name" class="flex flex-col overflow-hidden rounded-lg shadow-lg">
              <div class="bg-white px-6 py-8 sm:p-10 sm:pb-6">
                <div>
                  <h3 class="inline-flex rounded-full bg-indigo-100 px-4 py-1 text-base font-semibold text-indigo-600" id="tier-standard">{{ tier.name }}</h3>
                </div>
                <div class="mt-4 flex items-baseline text-6xl font-bold tracking-tight">
                  ${{ tier.priceMonthly }}
                  <span class="ml-1 text-2xl font-medium tracking-normal text-gray-500">/mo</span>
                </div>
                <p class="mt-5 text-lg text-gray-500">{{ tier.description }}</p>
              </div>
              <div class="flex flex-1 flex-col justify-between space-y-6 bg-gray-50 px-6 pt-6 pb-8 sm:p-10 sm:pt-6">
                <ul role="list" class="space-y-4">
                  <li v-for="feature in tier.features" :key="feature" class="flex items-start">
                    <div class="flex-shrink-0">
                      <CheckIcon class="h-6 w-6 text-green-500" aria-hidden="true" />
                    </div>
                    <p class="ml-3 text-base text-gray-700">{{ feature }}</p>
                  </li>
                </ul>
                <div class="rounded-md shadow">
                  <a :href="tier.href" class="flex items-center justify-center rounded-md border border-transparent bg-gray-800 px-5 py-3 text-base font-medium text-white hover:bg-gray-900" aria-describedby="tier-standard">Get started</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="relative mx-auto mt-4 max-w-7xl px-4 sm:px-6 lg:mt-5 lg:px-8">
        <div class="mx-auto max-w-md lg:max-w-5xl">
          <div class="rounded-lg bg-gray-100 px-6 py-8 sm:p-10 lg:flex lg:items-center">
            <div class="flex-1">
              <div>
                <h3 class="inline-flex rounded-full bg-white px-4 py-1 text-base font-semibold text-gray-800">API & Big Data</h3>
              </div>
              <div class="mt-4 text-lg text-gray-600">Integrate our data into your Data Science, Machine Learning & AI Flows <br><span class="font-semibold text-gray-900"> Starting from $749 p/m</span>.</div>
            </div>
            <div class="mt-6 rounded-md shadow lg:mt-0 lg:ml-10 lg:flex-shrink-0">
              <a href="/SaaS" class="flex items-center justify-center rounded-md border border-transparent bg-white px-5 py-3 text-base font-medium text-gray-900 hover:bg-gray-50">Learn More</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { CheckIcon } from '@heroicons/vue/24/outline'

const tiers = [
  {
    name: 'The Hobbyist',
    href: '#',
    priceMonthly: 249,
    description: 'Free Foverever. No credit card required.',
    features: [
      'Up to 250 Users',
      'Turnkey WL SaaS Framework',
      '100% WL & Rebrandable',
      'Billing & Subscription Management',
      'Authentication & Authorization',
      'User Management',
      'Admin Dashboard',
      'Embedable Frontend Into Any Website or App',
      'All Ad Platforms',
    ],
  },
  {
    name: 'WL SaaS Pro',
    href: '#',
    priceMonthly: 498,
    description: 'For small businesses and individuals.',
    features: [
      'Up to 750 Users',
      'Turnkey WL SaaS Framework',
      '100% WL & Rebrandable',
      'Billing & Subscription Management',
      'Authentication & Authorization',
      'User Management',
      'Admin Dashboard',
      'Embedable Frontend Into Any Website or App',
      'All Ad Platforms',
    ],
  },
]
</script>