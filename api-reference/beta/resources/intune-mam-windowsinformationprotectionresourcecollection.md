---
title: windowsInformationProtectionResourceCollection リソースの種類
description: Windows 情報保護のリソース コレクション
author: tfitzmac
ms.openlocfilehash: 96b3b36f40d1eeb88731f6f44ebec812a18fe713
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306889"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="a9c0f-103">windowsInformationProtectionResourceCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a9c0f-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="a9c0f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a9c0f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9c0f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9c0f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9c0f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9c0f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9c0f-107">Windows 情報保護のリソース コレクション</span><span class="sxs-lookup"><span data-stu-id="a9c0f-107">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="a9c0f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9c0f-108">Properties</span></span>
|<span data-ttu-id="a9c0f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9c0f-109">Property</span></span>|<span data-ttu-id="a9c0f-110">種類</span><span class="sxs-lookup"><span data-stu-id="a9c0f-110">Type</span></span>|<span data-ttu-id="a9c0f-111">説明</span><span class="sxs-lookup"><span data-stu-id="a9c0f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9c0f-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a9c0f-112">displayName</span></span>|<span data-ttu-id="a9c0f-113">文字列</span><span class="sxs-lookup"><span data-stu-id="a9c0f-113">String</span></span>|<span data-ttu-id="a9c0f-114">表示名</span><span class="sxs-lookup"><span data-stu-id="a9c0f-114">Display name</span></span>|
|<span data-ttu-id="a9c0f-115">リソース</span><span class="sxs-lookup"><span data-stu-id="a9c0f-115">resources</span></span>|<span data-ttu-id="a9c0f-116">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="a9c0f-116">String collection</span></span>|<span data-ttu-id="a9c0f-117">リソースのコレクション</span><span class="sxs-lookup"><span data-stu-id="a9c0f-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9c0f-118">関係</span><span class="sxs-lookup"><span data-stu-id="a9c0f-118">Relationships</span></span>
<span data-ttu-id="a9c0f-119">なし</span><span class="sxs-lookup"><span data-stu-id="a9c0f-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a9c0f-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a9c0f-120">JSON Representation</span></span>
<span data-ttu-id="a9c0f-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a9c0f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```





