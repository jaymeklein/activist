<template>
  <header
    ref="header"
    class="sticky top-0 z-10 w-full h-12 md:hidden duration-500 drop-shadow-md bg-light-layer-2 dark:bg-dark-layer-2"
  >
    <div class="h-full">
      <div class="flex justify-between h-full px-4 gap-2">
        <SearchBar
          @on-search-toggle="toggleSearchExpanded"
          class="my-1.5"
          :class="{ 'w-full': isSearchExpanded }"
          :location="SearchBarLocation.HEADER"
          :expanded="isSearchExpanded"
        />
        <IconActivist
          v-if="!isSearchExpanded"
          class="flex items-center w-6 h-8 absolute top-[0.3rem] m-auto left-0 right-0 overflow-clip"
        />
        <SidebarRight>
          <div class="flex-col space-y-2">
            <DropdownTheme
              class="w-full"
              :location="DropdownLocation.SIDEMENU"
            />
            <DropdownLanguage
              class="w-full"
              :location="DropdownLocation.SIDEMENU"
            />
            <DropdownCreate
              class="w-full"
              :location="DropdownLocation.SIDEMENU"
            />
            <DropdownInfo
              class="w-full"
              :location="DropdownLocation.SIDEMENU"
            />
            <DropdownUserOptions
              class="w-full"
              :location="DropdownLocation.SIDEMENU"
            />
          </div>
        </SidebarRight>
      </div>
    </div>
  </header>
</template>

<script setup lang="ts">
import { DropdownLocation, SearchBarLocation } from "~/types/location";

const isSearchExpanded = ref(false);

const toggleSearchExpanded = () => {
  isSearchExpanded.value = !isSearchExpanded.value;
};
</script>
