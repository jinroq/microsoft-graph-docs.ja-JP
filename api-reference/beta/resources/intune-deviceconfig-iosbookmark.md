---
title: iosBookmark リソースの種類
description: iOS URL ブックマーク
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1439fa41488a482e569f681c1e1864d63952ffc2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338071"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="4719f-103">iosBookmark リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4719f-103">iosBookmark resource type</span></span>

> <span data-ttu-id="4719f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4719f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4719f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4719f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4719f-106">iOS URL ブックマーク</span><span class="sxs-lookup"><span data-stu-id="4719f-106">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="4719f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4719f-107">Properties</span></span>
|<span data-ttu-id="4719f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4719f-108">Property</span></span>|<span data-ttu-id="4719f-109">型</span><span class="sxs-lookup"><span data-stu-id="4719f-109">Type</span></span>|<span data-ttu-id="4719f-110">説明</span><span class="sxs-lookup"><span data-stu-id="4719f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4719f-111">url</span><span class="sxs-lookup"><span data-stu-id="4719f-111">url</span></span>|<span data-ttu-id="4719f-112">String</span><span class="sxs-lookup"><span data-stu-id="4719f-112">String</span></span>|<span data-ttu-id="4719f-113">アクセスが許可されている URL</span><span class="sxs-lookup"><span data-stu-id="4719f-113">URL allowed to access</span></span>|
|<span data-ttu-id="4719f-114">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="4719f-114">bookmarkFolder</span></span>|<span data-ttu-id="4719f-115">String</span><span class="sxs-lookup"><span data-stu-id="4719f-115">String</span></span>|<span data-ttu-id="4719f-116">ブックマークを Safari で追加するフォルダー</span><span class="sxs-lookup"><span data-stu-id="4719f-116">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="4719f-117">displayName</span><span class="sxs-lookup"><span data-stu-id="4719f-117">displayName</span></span>|<span data-ttu-id="4719f-118">String</span><span class="sxs-lookup"><span data-stu-id="4719f-118">String</span></span>|<span data-ttu-id="4719f-119">ブックマークの表示名</span><span class="sxs-lookup"><span data-stu-id="4719f-119">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="4719f-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4719f-120">Relationships</span></span>
<span data-ttu-id="4719f-121">なし</span><span class="sxs-lookup"><span data-stu-id="4719f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4719f-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4719f-122">JSON Representation</span></span>
<span data-ttu-id="4719f-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4719f-123">Here is a JSON representation of the resource.</span></span>
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



