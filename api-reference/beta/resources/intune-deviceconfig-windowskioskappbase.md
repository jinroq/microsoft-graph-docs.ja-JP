---
title: windowsKioskAppBase リソースの種類
description: アプリケーションの型の基本クラス
author: tfitzmac
ms.openlocfilehash: 2afccff07d15fa1f2dfeff6a4ae9029494faa521
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307449"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="9f865-103">windowsKioskAppBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f865-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="9f865-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f865-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f865-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f865-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f865-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9f865-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f865-107">アプリケーションの型の基本クラス</span><span class="sxs-lookup"><span data-stu-id="9f865-107">The base class for a type of apps</span></span>
## <a name="properties"></a><span data-ttu-id="9f865-108">Properties</span><span class="sxs-lookup"><span data-stu-id="9f865-108">Properties</span></span>
|<span data-ttu-id="9f865-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f865-109">Property</span></span>|<span data-ttu-id="9f865-110">種類</span><span class="sxs-lookup"><span data-stu-id="9f865-110">Type</span></span>|<span data-ttu-id="9f865-111">説明</span><span class="sxs-lookup"><span data-stu-id="9f865-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f865-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="9f865-112">startLayoutTileSize</span></span>|[<span data-ttu-id="9f865-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="9f865-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="9f865-114">開始レイアウトのアプリケーションのタイルのサイズです。</span><span class="sxs-lookup"><span data-stu-id="9f865-114">The app tile size for the start layout.</span></span> <span data-ttu-id="9f865-115">可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。</span><span class="sxs-lookup"><span data-stu-id="9f865-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="9f865-116">名前</span><span class="sxs-lookup"><span data-stu-id="9f865-116">name</span></span>|<span data-ttu-id="9f865-117">String</span><span class="sxs-lookup"><span data-stu-id="9f865-117">String</span></span>|<span data-ttu-id="9f865-118">アプリケーションのフレンドリ名を表す</span><span class="sxs-lookup"><span data-stu-id="9f865-118">Represents the friendly name of an app</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f865-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9f865-119">Relationships</span></span>
<span data-ttu-id="9f865-120">なし</span><span class="sxs-lookup"><span data-stu-id="9f865-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9f865-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f865-121">JSON Representation</span></span>
<span data-ttu-id="9f865-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9f865-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String"
}
```





