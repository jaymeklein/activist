<template>
  <TooltipBase
    header="Restricted content"
    :text="$t('components.tooltip-sign-in.text')"
  >
    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 w-max">
      <BtnRouteInternal
        class="flex items-center justify-center truncate max-h-[40px]"
        label="_global.sign-in"
        linkTo="/auth/sign-in"
        :cta="true"
        fontSize="lg"
        :ariaLabel="$t('components.btn-route-internal.sign-in-aria-label')"
      />
      <BtnRouteInternal
        class="flex items-center justify-center truncate max-h-[40px]"
        label="_global.sign-up"
        linkTo="/auth/sign-up"
        :cta="true"
        fontSize="lg"
        :ariaLabel="$t('components.btn-route-internal.sign-up-aria-label')"
      />
    </div>
  </TooltipBase>
</template>
