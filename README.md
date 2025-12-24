# Ex09 Event Registration Web Application
## Date: 24.12.2025
## Reference No: 25002753

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
page1
import PropTypes from "prop-types";
import React from "react";
import { IphonePro } from "./IphonePro";
import { LiquidGlassRegular } from "./LiquidGlassRegular";
import { ScrollEdgeEffect } from "./ScrollEdgeEffect";
import { StatusBarIphone } from "./StatusBarIphone";
import { TabBarButton } from "./TabBarButton";
import { TabBarIphone } from "./TabBarIphone";
import { ToolbarTopIphone } from "./ToolbarTopIphone";

export const TabBar = ({
  splitSearch,
  className,
  scrollEdgeEffectEdgeTop = "scroll-edge-effect-soft.svg",
  scrollEdgeEffectEdgeBottom = "image.svg",
  tabBarIphoneLiquidGlassRegularBlur = "blur-11.svg",
  tabBarIphoneLiquidGlassRegularImg = "blur-12.svg",
  visible = true,
  statusBarIphoneLevels = "levels-2.svg",
  iphoneProIphoneProSilver = "image.png",
}) => {
  return (
    <div
      className={`w-[402px] top-10 h-[874px] relative ${splitSearch ? "left-10" : "left-[510px]"} ${className}`}
    >
      <div className="w-full flex left-0 flex-col items-center top-0 pt-[167px] pb-2.5 px-4 h-full overflow-hidden rounded-[50px] justify-center bg-colors-backgrounds-primary absolute">
        <div className="w-full flex self-stretch flex-col items-start grow gap-2.5 flex-1 px-0 py-2.5 relative">
          <div className="[font-family:'SF_Pro-Semibold',Helvetica] w-fit mt-[-1.00px] tracking-[0] text-[17px] text-colors-labels-primary font-normal text-center whitespace-nowrap leading-[22px] relative">
            Content area
          </div>
        </div>

        <ScrollEdgeEffect
          className="!object-cover !w-full"
          edge="top"
          edgeTop={scrollEdgeEffectEdgeTop}
        />
        <ScrollEdgeEffect
          className="!h-[110px] !object-cover !bottom-0 !w-full !top-[unset]"
          edge="bottom"
          edgeBottom={scrollEdgeEffectEdgeBottom}
        />
      </div>

      {!splitSearch && (
        <div className="flex w-full items-start justify-center pt-4 pb-[25px] px-[25px] absolute left-0 bottom-[7px]">
          <div className="flex items-start justify-center relative flex-1 grow">
            <LiquidGlassRegular
              blur="blur-9.svg"
              blurClassName="!left-[-26px] !top-[-26px]"
              className="!h-[calc(100%_+_8px)] !absolute !-left-1 !w-[calc(100%_+_8px)] !-top-1"
              mode="light"
              state="default"
            />
            <TabBarButton
              className="!left-[unset] !ml-[-7.33px] !flex-1 !grow !w-[unset] !top-[unset]"
              label="Tab 1"
              mode="light"
              selected
              symbol="􀟉"
            />
            <TabBarButton
              className="!left-[unset] !ml-[-7.33px] !flex-1 !grow !w-[unset] !top-[unset]"
              label="Tab 2"
              mode="light"
              selected={false}
              symbol="􀀁"
            />
            <TabBarButton
              className="!left-[unset] !ml-[-7.33px] !flex-1 !grow !w-[unset] !top-[unset]"
              label="Tab 3"
              mode="light"
              selected={false}
              symbol="􀛤"
            />
            <TabBarButton
              className="!left-[unset] !ml-[-7.33px] !flex-1 !grow !w-[unset] !top-[unset]"
              label="Tab 4"
              mode="light"
              selected={false}
              symbol="􀟇"
            />
          </div>
        </div>
      )}

      {splitSearch && (
        <TabBarIphone
          className="!absolute !left-0 !bottom-0 !w-full !top-[unset]"
          liquidGlassRegularBlur={tabBarIphoneLiquidGlassRegularBlur}
          liquidGlassRegularImg={tabBarIphoneLiquidGlassRegularImg}
          minimized={false}
          separateSearch
          tabBarButtonLabel="Tab 1"
          tabBarButtonLabel1="Tab 2"
          tabBarButtonLabel2="Tab 3"
          tabs="four"
        />
      )}

      {visible && (
        <ToolbarTopIphone
          buttonsTopLiquidGlassRegularBlur={
            splitSearch ? "blur-13.svg" : "blur-10.svg"
          }
          className="!absolute !left-0 !w-full !top-[62px]"
          hasLeading={false}
          showSubtitle={false}
          style="large-title"
          visible={false}
        />
      )}

      <StatusBarIphone
        className="!absolute !left-0 !w-full !top-0"
        levels={statusBarIphoneLevels}
        time="9:41"
      />
      <IphonePro
        className="!absolute !flex !left-0 !top-0"
        color="silver"
        iphoneProSilver={iphoneProIphoneProSilver}
        iphoneProSilverClassName="!mt-[-23px] !-ml-6 ![position:unset] !left-[unset] !top-[unset]"
      />
    </div>
  );
};

TabBar.propTypes = {
  splitSearch: PropTypes.bool,
  scrollEdgeEffectEdgeTop: PropTypes.string,
  scrollEdgeEffectEdgeBottom: PropTypes.string,
  tabBarIphoneLiquidGlassRegularBlur: PropTypes.string,
  tabBarIphoneLiquidGlassRegularImg: PropTypes.string,
  visible: PropTypes.bool,
  statusBarIphoneLevels: PropTypes.string,
  iphoneProIphoneProSilver: PropTypes.string,
};

page2
import React from "react";
import image4 from "./image-4.png";

export const Image = () => {
  return (
    <div className="w-[402px] h-[201px]">
      <img
        className="fixed top-0 left-0 w-[402px] h-[201px] aspect-[2] object-cover"
        alt="Image"
        src={image4}
      />
    </div>
  );
};

page3
import React from "react";
import image3 from "./image-3.png";

export const IphonePro = () => {
  return (
    <div className="bg-white w-full min-w-[402px] min-h-[874px] flex">
      <img
        className="w-[402px] h-[874px] aspect-[0.8] object-cover"
        alt="Image"
        src={image3}
      />
    </div>
  );
};

```
## OUTPUT:
![013](https://github.com/user-attachments/assets/64be4458-e528-44d9-bf09-8c750e1a3c48)


## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
