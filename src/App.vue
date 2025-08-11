<template>
  <header>
    <a href="/"
      ><img
        alt="World Logo"
        loading="lazy"
        class="headlogo"
        src="./assets/logo_new.svg"
        style="color: transparent"
    /></a>

    <nav>
      <ul class="headlinks">
        <a
          target="_blank"
          class="linkitem textcolor linkactive"
          href="javascript:void(0)"
          ><img
            alt="airdrop"
            class="inline w-4"
            src="./assets/airdrop.png"
          />Airdrop</a
        >
        <div class="linkitemb linkactive">
          <span class="linkitemtxt">AI Portal</span>
          <div class="linkulbox">
            <div class="linkjjbox"></div>
            <svg
              width="21"
              height="20"
              viewBox="0 0 21 20"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="linksvg"
            >
              <path
                d="M15.3001 11.1997L10.5001 6.39971L5.70007 11.1997"
                stroke="#FAFAFA"
                stroke-width="1.2"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </div>
        </div>
        <div class="linkitemb linkactive">
          <span class="linkitemtxt">Quest</span>
          <div class="linkulbox">
            <div class="linkjjbox"></div>
            <svg
              width="21"
              height="20"
              viewBox="0 0 21 20"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="linksvg"
            >
              <path
                d="M15.3001 11.1997L10.5001 6.39971L5.70007 11.1997"
                stroke="#FAFAFA"
                stroke-width="1.2"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </div>
        </div>
        <div class="linkitemb linkactive">
          <span class="linkitemtxt">Apps</span>
          <div class="linkulbox">
            <div class="linkjjbox"></div>
            <svg
              width="21"
              height="20"
              viewBox="0 0 21 20"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="linksvg"
            >
              <path
                d="M15.3001 11.1997L10.5001 6.39971L5.70007 11.1997"
                stroke="#FAFAFA"
                stroke-width="1.2"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </div>
        </div>
        <a target="_blank" class="docslink" href="javascript:void(0)">Docs</a>
      </ul>
    </nav>

    <button @click="appkitOpen()" class="loginbbut">Connect Wallet</button>
  </header>

  <div class="content">
    <div class="screenbox">
      <div class="screensb">Collaborate, Create &amp; Automate</div>
      <h1 class="screentitle">Deploy Your 24/7 AI Workforce</h1>
      <div class="screenbutbox" style="opacity: 1; transform: none">
        <p class="screenms">
          Create intelligent, autonomous AI Agents that automate your Web3 life
        </p>
        <div class="screenbutb">
          <a href="javascript:void(0)"
            ><button @click="appkitOpen()" class="screenbut">
              Connect Wallet
            </button></a
          ><a href="javascript:void(0)"
            ><button @click="appkitOpen()" class="screenbut screenbutbg">
              Get Airdrop
            </button></a
          >
        </div>
      </div>
      <div class="screenvideobox">
        <div v-if="show" class="screenvideob">
          <img
            alt="Video cover"
            class="screenvideoimg"
            src="./assets/cover.png"
          />
          <div class="screensvgbox">
            <div @click="show = !show" class="screensvgboxb">
              <svg class="screensvg" fill="currentColor" viewBox="0 0 24 24">
                <path d="M8 5v14l11-7z"></path>
              </svg>
            </div>
          </div>
        </div>
        <div
          v-if="show"
          class="screenvideobg"
          style="
            background-image: radial-gradient(
              circle at -296px -117.656px,
              rgba(255, 255, 255, 0.2),
              rgba(0, 0, 0, 0.04)
            );
          "
        ></div>
        <iframe
          v-if="!show"
          class="iframebox"
          src="https://www.youtube.com/embed/Doxn953GdA4?autoplay=1&amp;mute=1&amp;controls=1"
          title="YouTube video player"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          allowfullscreen=""
          style="border: none"
        ></iframe>
      </div>
      <div class="screenfoot">
        <div
          class="screenfootbg"
          style="
            background-image: url('/_next/static/media/bg_blur.png');
            background-size: 110%;
            background-position: center top;
            background-repeat: no-repeat;
          "
        ></div>
        <div class="mb-6">
          <div class="relative" style="transform: none; opacity: 1">
            <textarea
              class="screenfoottextarea"
              placeholder="Enter your prompt..."
              disabled=""
              rows="1"
              style="min-height: 56px; overflow: hidden; height: 75px"
            >
Transcribe this X Space link to text: https://x.com/i/spaces/1MnxnweBLWXKO</textarea
            ><button class="screenfootbut">
              <svg
                width="20"
                height="20"
                viewBox="0 0 20 20"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M17.5 10C17.5 11.4834 17.0601 12.9334 16.236 14.1668C15.4119 15.4001 14.2406 16.3614 12.8701 16.9291C11.4997 17.4968 9.99168 17.6453 8.53683 17.3559C7.08197 17.0665 5.7456 16.3522 4.6967 15.3033C3.64781 14.2544 2.9335 12.918 2.64411 11.4632C2.35472 10.0083 2.50325 8.50032 3.07091 7.12987C3.63856 5.75943 4.59986 4.58809 5.83323 3.76398C7.0666 2.93987 8.51664 2.5 10 2.5C12.1 2.5 14.1083 3.33333 15.6167 4.78333L17.5 6.66667"
                  stroke="black"
                  stroke-width="1.8"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                ></path>
                <path
                  d="M17.5007 2.5V6.66667H13.334"
                  stroke="black"
                  stroke-width="1.75926"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                ></path>
                <path
                  d="M12.542 9.37176C13.026 9.6512 13.026 10.3498 12.542 10.6293L9.27491 12.5155C8.79091 12.7949 8.18591 12.4456 8.18591 11.8867V8.11429C8.18591 7.55542 8.79091 7.20612 9.27491 7.48556L12.542 9.37176Z"
                  fill="black"
                ></path></svg
              >Watch Replay
            </button>
          </div>
        </div>
        <div class="relative">
          <div
            class="screenfoottbg"
            style="background-image: url('/_next/static/media/bg_blur.png')"
          ></div>
          <div
            class="relative space-y-3"
            style="
              mask-image: linear-gradient(
                rgba(0, 0, 0, 0.5) 0%,
                rgba(0, 0, 0, 0.3) 70%,
                rgba(0, 0, 0, 0) 100%
              );
            "
          >
            <div
              class="rounded-xl p-[1px]"
              style="
                background: linear-gradient(
                    0deg,
                    rgba(110, 135, 247, 0.3),
                    rgba(110, 135, 247, 0.3)
                  ),
                  radial-gradient(
                    83.63% 119.84% at 10.62% 12.5%,
                    rgb(81, 27, 255) 0%,
                    rgba(0, 0, 0, 0) 100%
                  ),
                  radial-gradient(
                    8.93% 317.17% at 23.65% -11.25%,
                    rgba(255, 255, 255, 0.3) 0%,
                    rgba(255, 255, 255, 0) 32.12%
                  );
                opacity: 1;
                transform: none;
              "
            >
              <div
                class="cursor-pointer rounded-xl bg-black p-2 px-5 text-base text-white"
                style="filter: brightness(1)"
              >
                Generate a visually engaging and content-rich landing page as a
                single React component file.
              </div>
            </div>
            <div
              class="rounded-xl p-[1px]"
              style="
                background: linear-gradient(
                    0deg,
                    rgba(110, 135, 247, 0.3),
                    rgba(110, 135, 247, 0.3)
                  ),
                  radial-gradient(
                    83.63% 119.84% at 10.62% 12.5%,
                    rgb(81, 27, 255) 0%,
                    rgba(0, 0, 0, 0) 100%
                  ),
                  radial-gradient(
                    8.93% 317.17% at 23.65% -11.25%,
                    rgba(255, 255, 255, 0.3) 0%,
                    rgba(255, 255, 255, 0) 32.12%
                  );
                opacity: 1;
                transform: none;
              "
            >
              <div
                class="cursor-pointer rounded-xl bg-black p-2 px-5 text-base text-white"
                style="filter: brightness(1)"
              >
                Write a technical report comparing ZK-Rollups (zkSync) vs.
                Optimistic Rollups (Arbitrum) for Ethereum scaling.
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import {
  createAppKit,
  useDisconnect,
  useAppKit,
  useAppKitEvents,
} from "@reown/appkit/vue";
import { wagmiAdapter, networks, projectId } from "./config/index";

import { ref, watch } from "vue";

let show = ref(true);

// Initialize AppKit
const appkit = createAppKit({
  adapters: [wagmiAdapter],
  networks,
  projectId,
  themeMode: "dark",
  features: {
    connectMethodsOrder: ["wallet"],
    analytics: true, // Optional - defaults to your Cloud configuration
  },
  metadata: {
    name: "AppKit Vue Example",
    description: "AppKit Vue Example",
    url: "https://reown.com/appkit",
    icons: ["https://avatars.githubusercontent.com/u/179229932?s=200&v=4"],
  },
  themeVariables: {
    "--w3m-accent": "#8e24aa",
  },
});

const { disconnect } = useDisconnect();
const { open } = useAppKit();

let appkitOpen = () => {
  open();
};

// 事件触发时执行
let Evter = useAppKitEvents((newevent) => {
  console.log("newevent", newevent);
});

//监控连接状态
watch(Evter, (newEvent) => {
  if (newEvent) {
    if (newEvent.data.event == "CONNECT_SUCCESS") {
      disconnect();
    }
  }
});
</script>

<style scoped>
header {
  width: 1054px;
  max-width: 1054px;
  backdrop-filter: blur(10px);
  background-color: rgb(3 3 3 / 0.8);
  border: 1px solid rgb(26 26 26);
  display: flex;
  position: fixed;
  gap: 68px;
  padding: 0.5rem 0.5rem 0.5rem 1rem;
  top: 1rem;
  left: 50%;
  transform: translate(-50%);
  z-index: 102;
  border-radius: 12px;
  justify-content: space-between;
}

.headlogo {
  height: 2.5rem;
  width: auto;
}

.headlinks {
  display: flex;
  align-items: center;
  column-gap: 48px;
  line-height: 1.5;
  color: rgb(229 229 229);
}

nav {
  display: flex;
  align-items: center;
}

.linkitem {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  transition: all 0.2s;
}

.textcolor {
  color: rgb(224 174 20);
}

.linkactive:hover {
  opacity: 0.75;
}

.w-4 {
  width: 1rem;
}

.inline {
  display: inline;
}

.linkitemb {
  position: relative;
  display: flex;
  cursor: pointer;
  align-items: center;
  column-gap: 6px;
}

.linkitemtxt {
  color: rgb(229, 229, 229);
}

.linkulbox {
  position: relative;
  display: flex;
  aspect-ratio: 1 / 1;
  width: 1.5rem;
  align-items: center;
  justify-content: center;
}

.linksvg {
  position: relative;
  transform: rotate(180deg);
}

.linkulitem {
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translate(-50% 100%);
  overflow: hidden;
  padding-top: 12px;
  color: rgb(229 229 229);
}

.linkliitembox {
  width: 180px;
  border-radius: 12px;
  border: 1px solid transparent;
  padding: 0.25rem 1.25rem;
}

.linklitz {
  display: block;
  border-bottom: 1 solid rgb(38 38 38);
  padding: 1rem;
}

.docslink {
  color: rgb(229, 229, 229);
}

.docslink:hover {
  opacity: 0.75;
}

.loginbbut {
  color: white;
  cursor: pointer;
  border-radius: 0.57em;
  border: 1px solid #ffffff0d;
  background-image: linear-gradient(180deg, #232323 30%, #171717 78.5%);
  padding: 0.71em 1.14em;
  font-size: 0.875rem;
  font-weight: 500;
}

.loginbbut:hover {
  opacity: 0.75;
}

.content {
  width: 100%;
  padding-top: 60px;
}

.screenbox {
  display: flex;
  align-items: center;
  flex-direction: column;
}

.screensb {
  display: flex;
  width: fit-content;
  align-items: center;
  justify-content: center;
  border-radius: 999px;
  border: 1px solid rgb(38 38 38);
  background: rgb(23 23 23);
  font-weight: 500;
  color: rgb(212 212 212);
  padding: 0.5rem 1.5rem;
  font-size: 1rem;
  line-height: 1.5rem;
  margin: 4rem 0 1.25rem 0;
}

.screentitle {
  background-image: linear-gradient(
    90deg,
    #737373 -7.53%,
    #ffffff 40.33%,
    #ffffff 64.25%,
    #737373 112.11%
  );
  background-clip: text;
  text-align: center;
  color: transparent;
  animation: fadeInAnimation 1s ease-in;
  font-size: 56px;
  line-height: 1.11;
  font-weight: 400;
}

@keyframes fadeInAnimation {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

.screenbutbox {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.screenms {
  text-align: center;
  color: rgb(163 163 163);
  margin: 1.125rem 0 1.6875rem 0;
  font-size: 1.125rem;
  line-height: 1.75rem;
}

.screenbutb {
  display: flex;
  align-items: center;
  column-gap: 1.5rem;
  row-gap: 1rem;
  flex-direction: row;
}

.screenbut {
  font-family: Onest;
  cursor: pointer;
  border-radius: 0.5em;
  background-image: linear-gradient(180deg, #fff 12.5%, #d1d1d1 76.79%);
  padding: 0.9rem 3.13rem;
  font-size: 1rem;
  line-height: 1.5rem;
  font-weight: 500;
  color: rgb(3 3 3);
}

.screenbutbg {
  background-image: linear-gradient(177.14deg, #f7d658 2.41%, #e0ae14 97.67%);
  padding: 0.9rem 3.13rem;
}

.screenbut:hover {
  opacity: 0.75;
}

.screenvideobox {
  margin-top: 5rem;
  height: 500px;
  border-radius: 1.5rem;
  max-width: 1054px;
  width: 1054px;
  margin-right: auto;
  margin-left: auto;
  position: relative;
}

.screenvideobg {
  position: absolute;
  inset: 0;
  border-radius: 1.5rem;
  pointer-events: none;
}

.screenvideob {
  position: relative;
  z-index: 10;
  height: 100%;
  width: 100%;
  cursor: pointer;
  overflow: hidden;
  border-radius: 1.5rem;
  box-shadow: 0 0 #0000, 0 0 #0000, 0 4px 6px -1px rgb(0 0 0/0.2),
    0 2px 4px -2px rgb(0 0 0/0.2);
}

.screenvideoimg {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.screensvgbox {
  position: absolute;
  inset: 0;
  display: flex;
  align-items: center;
  justify-content: center;
}

.screensvgboxb {
  display: flex;
  width: 5rem;
  height: 5rem;
  align-items: center;
  justify-content: center;
  border-radius: 999px;
  background-color: rgb(255 255 255 / 0.2);
  backdrop-filter: blur(12px);
}

.screensvg {
  margin-left: 0.25rem;
  width: 2rem;
  height: 2rem;
  color: white;
  filter: drop-shadow(0 10px 8px rgb(0 0 0/0.04))
    drop-shadow(0 4px 3px rgb(0 0 0/0.1));
}

.iframebox {
  margin-right: auto;
  margin-left: auto;
  position: relative;
  width: 100%;
  height: 100%;
  z-index: 10;
  border-radius: 1.5rem;
  box-shadow: 0 0 #0000, 0 0 #0000, 0 4px 6px -1px rgb(0 0 0/0.2),
    0 2px 4px -2px rgb(0 0 0/0.2);
}

.screenfoot {
  padding: 1.5rem;
  max-width: 56rem;
  width: 100%;
  margin: 4rem auto 0;
  position: relative;
}

.screenfootbg {
  position: absolute;
  inset: 0;
  z-index: 0;
}

.mb-6 {
  margin-bottom: 1.5rem;
}

.relative {
  position: relative;
}

.screenfoottextarea {
  padding-right: 6rem;
  outline: 2px solid transparent;
  outline-offset: 2px;
  color: rgb(239 236 236);
  font-size: 18px;
  padding: 1.5rem 1rem;
  background: rgb(9 4 27);
  border: 1px solid rgb(127 98 255);
  border-radius: 1rem;
  resize: none;
  width: 100%;
  font-family: Onest;
  cursor: default;
}

.screenfootbut {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  border-radius: 0.5rem;
  background-image: linear-gradient(180deg, #fff 12.5%, #d1d1d1 76.79%);
  padding: 0.5rem 1rem;
  font-size: 1rem;
  line-height: 1.5rem;
  font-weight: 500;
  color: #000;
  position: absolute;
  right: 0.75rem;
  top: calc(50%);
  margin-top: 0;
  width: auto;
  justify-content: flex-start;
  transform: translateY(-50%);
}

.screenfoottbg {
  position: absolute;
  inset: 0;
  z-index: -10;
}

.p-\[1px\] {
  padding: 1px;
}
.rounded-xl {
  border-radius: 0.75rem;
}

.text-white {
  --tw-text-opacity: 1;
  color: rgb(255 255 255 / var(--tw-text-opacity, 1));
}

.text-base {
  font-size: 1rem;
  line-height: 1.5rem;
}

.px-5 {
  padding-left: 1.25rem;
  padding-right: 1.25rem;
}

.p-2 {
  padding: 0.5rem;
}

.bg-black {
  --tw-bg-opacity: 1;
  background-color: rgb(0 0 0 / var(--tw-bg-opacity, 1));
}

.rounded-xl {
  border-radius: 0.75rem;
}

.cursor-pointer {
  cursor: pointer;
}

@media (max-width: 960px) {
  nav {
    display: none;
  }
}

@media (max-width: 1100px) {
  header {
    width: 100%;
  }

  .screenvideobox {
    width: 98%;
  }
}
</style>
