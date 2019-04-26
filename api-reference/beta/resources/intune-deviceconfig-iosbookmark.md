---
title: iosbookmark リソースの種類
description: iOS URL ブックマーク
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5231ccbae496e310e414c6429190e0b4d53cbaa7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556040"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="35ee6-103">iosbookmark リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35ee6-103">iosBookmark resource type</span></span>

> <span data-ttu-id="35ee6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35ee6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35ee6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="35ee6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35ee6-106">iOS URL ブックマーク</span><span class="sxs-lookup"><span data-stu-id="35ee6-106">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="35ee6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35ee6-107">Properties</span></span>
|<span data-ttu-id="35ee6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35ee6-108">Property</span></span>|<span data-ttu-id="35ee6-109">型</span><span class="sxs-lookup"><span data-stu-id="35ee6-109">Type</span></span>|<span data-ttu-id="35ee6-110">説明</span><span class="sxs-lookup"><span data-stu-id="35ee6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35ee6-111">url</span><span class="sxs-lookup"><span data-stu-id="35ee6-111">url</span></span>|<span data-ttu-id="35ee6-112">String</span><span class="sxs-lookup"><span data-stu-id="35ee6-112">String</span></span>|<span data-ttu-id="35ee6-113">アクセスが許可されている URL</span><span class="sxs-lookup"><span data-stu-id="35ee6-113">URL allowed to access</span></span>|
|<span data-ttu-id="35ee6-114">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="35ee6-114">bookmarkFolder</span></span>|<span data-ttu-id="35ee6-115">String</span><span class="sxs-lookup"><span data-stu-id="35ee6-115">String</span></span>|<span data-ttu-id="35ee6-116">ブックマークを Safari で追加するフォルダー</span><span class="sxs-lookup"><span data-stu-id="35ee6-116">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="35ee6-117">displayName</span><span class="sxs-lookup"><span data-stu-id="35ee6-117">displayName</span></span>|<span data-ttu-id="35ee6-118">String</span><span class="sxs-lookup"><span data-stu-id="35ee6-118">String</span></span>|<span data-ttu-id="35ee6-119">ブックマークの表示名</span><span class="sxs-lookup"><span data-stu-id="35ee6-119">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="35ee6-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35ee6-120">Relationships</span></span>
<span data-ttu-id="35ee6-121">なし</span><span class="sxs-lookup"><span data-stu-id="35ee6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35ee6-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35ee6-122">JSON Representation</span></span>
<span data-ttu-id="35ee6-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="35ee6-123">Here is a JSON representation of the resource.</span></span>
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





