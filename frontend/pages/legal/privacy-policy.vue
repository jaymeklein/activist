<template>
  <div
    class="text-light-text dark:text-dark-text bg-light-layer-0 dark:bg-dark-layer-0"
  >
    <Head>
      <Title>{{ $t("pages.legal.privacy-policy.title") }}</Title>
    </Head>
    <PageDocs
      imgURL="/images/content_pages/icons/bootstrap_shield_check"
      imgAltText="pages.legal._global.privacy-policy-alt-text"
    >
      <h1 class="pb-2 font-bold responsive-h1">
        {{ $t("_global.privacy-policy") }}
      </h1>
      <p
        class="responsive-h4 text-light-distinct-text dark:text-dark-distinct-text"
      >
        {{ $t("pages.legal.privacy-policy.last-updated") }}
      </p>
      <p>
        {{ $t("pages.legal.privacy-policy.section-1-paragraph-1") }}
      </p>
      <p>
        {{ $t("pages.legal.privacy-policy.section-1-paragraph-2") }}
      </p>
      <p>
        {{ $t("pages.legal.privacy-policy.section-1-paragraph-3") }}
      </p>
      <h2 class="font-bold responsive-h3">
        {{ $t("pages.legal.privacy-policy.section-2-subheader") }}
      </h2>
      <p>
        {{ $t("pages.legal.privacy-policy.section-2-paragraph-1") }}
      </p>
      <h2 class="font-bold responsive-h3">
        {{ $t("pages.legal.privacy-policy.section-3-subheader") }}
      </h2>
      <p>
        {{ $t("pages.legal.privacy-policy.section-3-paragraph-1") }}
      </p>
      <h2 class="font-bold responsive-h3">
        {{ $t("pages.legal.privacy-policy.section-4-subheader") }}
      </h2>
      <p>
        {{ $t("pages.legal.privacy-policy.section-4-paragraph-1") }}
      </p>
      <h2 class="font-bold responsive-h3">
        {{ $t("pages.legal.privacy-policy.section-5-subheader") }}
      </h2>
      <p>
        {{ $t("pages.legal.privacy-policy.section-5-paragraph-1") }}
      </p>
      <p>
        {{ $t("pages.legal.privacy-policy.section-5-paragraph-2") }}
      </p>
      <h2 class="font-bold responsive-h3">
        {{ $t("pages.legal.privacy-policy.section-6-subheader") }}
      </h2>
      <p>
        {{ $t("pages.legal.privacy-policy.section-6-paragraph-1") }}
      </p>
      <h2 class="font-bold responsive-h3">
        {{ $t("pages.legal.privacy-policy.section-7-subheader") }}
      </h2>
      <p>
        {{ $t("pages.legal.privacy-policy.section-7-paragraph-1") }}
      </p>
      <PageCommunityFooter>
        <BtnRouteInternal
          class="w-full"
          :cta="false"
          label="components.btn-route-internal.return-home"
          linkTo="/"
          fontSize="lg"
          ariaLabel="components.btn-route-internal.return-home-aria-label"
        />
      </PageCommunityFooter>
    </PageDocs>
  </div>
</template>
