---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
ms.openlocfilehash: 16d191bb53f7546598b7869e8bc28be07cc4f604
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070893"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="d21f8-103">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d21f8-103">appListItem resource type</span></span>

> <span data-ttu-id="d21f8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d21f8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d21f8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d21f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d21f8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d21f8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d21f8-107">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="d21f8-107">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="d21f8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d21f8-108">Properties</span></span>
|<span data-ttu-id="d21f8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d21f8-109">Property</span></span>|<span data-ttu-id="d21f8-110">型</span><span class="sxs-lookup"><span data-stu-id="d21f8-110">Type</span></span>|<span data-ttu-id="d21f8-111">説明</span><span class="sxs-lookup"><span data-stu-id="d21f8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d21f8-112">名前</span><span class="sxs-lookup"><span data-stu-id="d21f8-112">name</span></span>|<span data-ttu-id="d21f8-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d21f8-113">String</span></span>|<span data-ttu-id="d21f8-114">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="d21f8-114">The application name</span></span>|
|<span data-ttu-id="d21f8-115">発行元</span><span class="sxs-lookup"><span data-stu-id="d21f8-115">publisher</span></span>|<span data-ttu-id="d21f8-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d21f8-116">String</span></span>|<span data-ttu-id="d21f8-117">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="d21f8-117">The publisher of the application</span></span>|
|<span data-ttu-id="d21f8-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d21f8-118">appStoreUrl</span></span>|<span data-ttu-id="d21f8-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d21f8-119">String</span></span>|<span data-ttu-id="d21f8-120">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="d21f8-120">The Store URL of the application</span></span>|
|<span data-ttu-id="d21f8-121">appId</span><span class="sxs-lookup"><span data-stu-id="d21f8-121">appId</span></span>|<span data-ttu-id="d21f8-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d21f8-122">String</span></span>|<span data-ttu-id="d21f8-123">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="d21f8-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="d21f8-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d21f8-124">Relationships</span></span>
<span data-ttu-id="d21f8-125">なし</span><span class="sxs-lookup"><span data-stu-id="d21f8-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d21f8-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d21f8-126">JSON Representation</span></span>
<span data-ttu-id="d21f8-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d21f8-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```





