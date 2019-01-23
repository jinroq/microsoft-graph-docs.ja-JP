---
title: iosBookmark リソースの種類
description: iOS の URL のブックマーク
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e95f3bfd40bdf5ca5782aa9233a020623d32d6a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395910"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="bb95c-103">iosBookmark リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb95c-103">iosBookmark resource type</span></span>

> <span data-ttu-id="bb95c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bb95c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bb95c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb95c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb95c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb95c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb95c-107">iOS の URL のブックマーク</span><span class="sxs-lookup"><span data-stu-id="bb95c-107">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="bb95c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb95c-108">Properties</span></span>
|<span data-ttu-id="bb95c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb95c-109">Property</span></span>|<span data-ttu-id="bb95c-110">型</span><span class="sxs-lookup"><span data-stu-id="bb95c-110">Type</span></span>|<span data-ttu-id="bb95c-111">説明</span><span class="sxs-lookup"><span data-stu-id="bb95c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb95c-112">url</span><span class="sxs-lookup"><span data-stu-id="bb95c-112">url</span></span>|<span data-ttu-id="bb95c-113">String</span><span class="sxs-lookup"><span data-stu-id="bb95c-113">String</span></span>|<span data-ttu-id="bb95c-114">URL のアクセスを許可</span><span class="sxs-lookup"><span data-stu-id="bb95c-114">URL allowed to access</span></span>|
|<span data-ttu-id="bb95c-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="bb95c-115">bookmarkFolder</span></span>|<span data-ttu-id="bb95c-116">String</span><span class="sxs-lookup"><span data-stu-id="bb95c-116">String</span></span>|<span data-ttu-id="bb95c-117">フォルダーには、Safari でブックマークを追加します。</span><span class="sxs-lookup"><span data-stu-id="bb95c-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="bb95c-118">displayName</span><span class="sxs-lookup"><span data-stu-id="bb95c-118">displayName</span></span>|<span data-ttu-id="bb95c-119">String</span><span class="sxs-lookup"><span data-stu-id="bb95c-119">String</span></span>|<span data-ttu-id="bb95c-120">ブックマークの表示名</span><span class="sxs-lookup"><span data-stu-id="bb95c-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb95c-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb95c-121">Relationships</span></span>
<span data-ttu-id="bb95c-122">なし</span><span class="sxs-lookup"><span data-stu-id="bb95c-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb95c-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb95c-123">JSON Representation</span></span>
<span data-ttu-id="bb95c-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bb95c-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosBookmark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosBookmark",
  "url": "String",
  "bookmarkFolder": "String",
  "displayName": "String"
}
```




