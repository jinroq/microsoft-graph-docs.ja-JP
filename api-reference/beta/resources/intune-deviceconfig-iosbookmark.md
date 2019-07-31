---
title: iosBookmark リソースの種類
description: iOS URL ブックマーク
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9310ffe3a664b3fc02e9f498a2c5312dc6683b53
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004345"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="7bae8-103">iosBookmark リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7bae8-103">iosBookmark resource type</span></span>

> <span data-ttu-id="7bae8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7bae8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bae8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7bae8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bae8-106">iOS URL ブックマーク</span><span class="sxs-lookup"><span data-stu-id="7bae8-106">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="7bae8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7bae8-107">Properties</span></span>
|<span data-ttu-id="7bae8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7bae8-108">Property</span></span>|<span data-ttu-id="7bae8-109">型</span><span class="sxs-lookup"><span data-stu-id="7bae8-109">Type</span></span>|<span data-ttu-id="7bae8-110">説明</span><span class="sxs-lookup"><span data-stu-id="7bae8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bae8-111">url</span><span class="sxs-lookup"><span data-stu-id="7bae8-111">url</span></span>|<span data-ttu-id="7bae8-112">String</span><span class="sxs-lookup"><span data-stu-id="7bae8-112">String</span></span>|<span data-ttu-id="7bae8-113">アクセスが許可されている URL</span><span class="sxs-lookup"><span data-stu-id="7bae8-113">URL allowed to access</span></span>|
|<span data-ttu-id="7bae8-114">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="7bae8-114">bookmarkFolder</span></span>|<span data-ttu-id="7bae8-115">String</span><span class="sxs-lookup"><span data-stu-id="7bae8-115">String</span></span>|<span data-ttu-id="7bae8-116">ブックマークを Safari で追加するフォルダー</span><span class="sxs-lookup"><span data-stu-id="7bae8-116">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="7bae8-117">displayName</span><span class="sxs-lookup"><span data-stu-id="7bae8-117">displayName</span></span>|<span data-ttu-id="7bae8-118">String</span><span class="sxs-lookup"><span data-stu-id="7bae8-118">String</span></span>|<span data-ttu-id="7bae8-119">ブックマークの表示名</span><span class="sxs-lookup"><span data-stu-id="7bae8-119">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bae8-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7bae8-120">Relationships</span></span>
<span data-ttu-id="7bae8-121">なし</span><span class="sxs-lookup"><span data-stu-id="7bae8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bae8-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7bae8-122">JSON Representation</span></span>
<span data-ttu-id="7bae8-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7bae8-123">Here is a JSON representation of the resource.</span></span>
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





