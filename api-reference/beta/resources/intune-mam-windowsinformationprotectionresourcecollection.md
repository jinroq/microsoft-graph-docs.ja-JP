---
title: windowsInformationProtectionResourceCollection リソースの種類
description: Windows 情報保護のリソース コレクション
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2a65704170c048f4aae66876f11ef8543c7b09e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933009"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="f0fc0-103">windowsInformationProtectionResourceCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f0fc0-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="f0fc0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f0fc0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0fc0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0fc0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0fc0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f0fc0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0fc0-107">Windows 情報保護のリソース コレクション</span><span class="sxs-lookup"><span data-stu-id="f0fc0-107">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="f0fc0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0fc0-108">Properties</span></span>
|<span data-ttu-id="f0fc0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0fc0-109">Property</span></span>|<span data-ttu-id="f0fc0-110">種類</span><span class="sxs-lookup"><span data-stu-id="f0fc0-110">Type</span></span>|<span data-ttu-id="f0fc0-111">説明</span><span class="sxs-lookup"><span data-stu-id="f0fc0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0fc0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f0fc0-112">displayName</span></span>|<span data-ttu-id="f0fc0-113">文字列</span><span class="sxs-lookup"><span data-stu-id="f0fc0-113">String</span></span>|<span data-ttu-id="f0fc0-114">表示名</span><span class="sxs-lookup"><span data-stu-id="f0fc0-114">Display name</span></span>|
|<span data-ttu-id="f0fc0-115">リソース</span><span class="sxs-lookup"><span data-stu-id="f0fc0-115">resources</span></span>|<span data-ttu-id="f0fc0-116">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f0fc0-116">String collection</span></span>|<span data-ttu-id="f0fc0-117">リソースのコレクション</span><span class="sxs-lookup"><span data-stu-id="f0fc0-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0fc0-118">関係</span><span class="sxs-lookup"><span data-stu-id="f0fc0-118">Relationships</span></span>
<span data-ttu-id="f0fc0-119">なし</span><span class="sxs-lookup"><span data-stu-id="f0fc0-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f0fc0-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f0fc0-120">JSON Representation</span></span>
<span data-ttu-id="f0fc0-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f0fc0-121">Here is a JSON representation of the resource.</span></span>
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





