---
title: windowsKioskDesktopApp リソースの種類
description: アプリケーションの型の基本クラス
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a9b808bfd67e1b14e0b11fe84da48b77b4d965ba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947331"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="a41f2-103">windowsKioskDesktopApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a41f2-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="a41f2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a41f2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a41f2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a41f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a41f2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a41f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a41f2-107">アプリケーションの型の基本クラス</span><span class="sxs-lookup"><span data-stu-id="a41f2-107">The base class for a type of apps</span></span>

<span data-ttu-id="a41f2-108">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a41f2-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a41f2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a41f2-109">Properties</span></span>
|<span data-ttu-id="a41f2-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a41f2-110">Property</span></span>|<span data-ttu-id="a41f2-111">型</span><span class="sxs-lookup"><span data-stu-id="a41f2-111">Type</span></span>|<span data-ttu-id="a41f2-112">説明</span><span class="sxs-lookup"><span data-stu-id="a41f2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a41f2-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="a41f2-113">startLayoutTileSize</span></span>|[<span data-ttu-id="a41f2-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="a41f2-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="a41f2-115">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承される開始レイアウトのアプリケーションのタイルのサイズです。</span><span class="sxs-lookup"><span data-stu-id="a41f2-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="a41f2-116">可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。</span><span class="sxs-lookup"><span data-stu-id="a41f2-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="a41f2-117">名前</span><span class="sxs-lookup"><span data-stu-id="a41f2-117">name</span></span>|<span data-ttu-id="a41f2-118">String</span><span class="sxs-lookup"><span data-stu-id="a41f2-118">String</span></span>|<span data-ttu-id="a41f2-119">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承される、アプリケーションのフレンドリ名を表す</span><span class="sxs-lookup"><span data-stu-id="a41f2-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="a41f2-120">path</span><span class="sxs-lookup"><span data-stu-id="a41f2-120">path</span></span>|<span data-ttu-id="a41f2-121">String</span><span class="sxs-lookup"><span data-stu-id="a41f2-121">String</span></span>|<span data-ttu-id="a41f2-122">デスクトップ アプリケーションのパスを定義します。</span><span class="sxs-lookup"><span data-stu-id="a41f2-122">Define the path of a desktop app</span></span>|
|<span data-ttu-id="a41f2-123">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="a41f2-123">desktopApplicationId</span></span>|<span data-ttu-id="a41f2-124">String</span><span class="sxs-lookup"><span data-stu-id="a41f2-124">String</span></span>|<span data-ttu-id="a41f2-125">アプリケーションの DesktopApplicationID を定義します。</span><span class="sxs-lookup"><span data-stu-id="a41f2-125">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="a41f2-126">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="a41f2-126">desktopApplicationLinkPath</span></span>|<span data-ttu-id="a41f2-127">String</span><span class="sxs-lookup"><span data-stu-id="a41f2-127">String</span></span>|<span data-ttu-id="a41f2-128">アプリケーションの DesktopApplicationLinkPath を定義します。</span><span class="sxs-lookup"><span data-stu-id="a41f2-128">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="a41f2-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a41f2-129">Relationships</span></span>
<span data-ttu-id="a41f2-130">なし</span><span class="sxs-lookup"><span data-stu-id="a41f2-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a41f2-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a41f2-131">JSON Representation</span></span>
<span data-ttu-id="a41f2-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a41f2-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskDesktopApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```





