---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 492828fdef95815704083ec8f496e38a10dc3559
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923335"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="34349-103">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="34349-103">appListItem resource type</span></span>

> <span data-ttu-id="34349-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="34349-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34349-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34349-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34349-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="34349-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34349-107">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="34349-107">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="34349-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34349-108">Properties</span></span>
|<span data-ttu-id="34349-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34349-109">Property</span></span>|<span data-ttu-id="34349-110">種類</span><span class="sxs-lookup"><span data-stu-id="34349-110">Type</span></span>|<span data-ttu-id="34349-111">説明</span><span class="sxs-lookup"><span data-stu-id="34349-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34349-112">名前</span><span class="sxs-lookup"><span data-stu-id="34349-112">name</span></span>|<span data-ttu-id="34349-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="34349-113">String</span></span>|<span data-ttu-id="34349-114">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="34349-114">The application name</span></span>|
|<span data-ttu-id="34349-115">発行元</span><span class="sxs-lookup"><span data-stu-id="34349-115">publisher</span></span>|<span data-ttu-id="34349-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="34349-116">String</span></span>|<span data-ttu-id="34349-117">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="34349-117">The publisher of the application</span></span>|
|<span data-ttu-id="34349-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="34349-118">appStoreUrl</span></span>|<span data-ttu-id="34349-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="34349-119">String</span></span>|<span data-ttu-id="34349-120">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="34349-120">The Store URL of the application</span></span>|
|<span data-ttu-id="34349-121">appId</span><span class="sxs-lookup"><span data-stu-id="34349-121">appId</span></span>|<span data-ttu-id="34349-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="34349-122">String</span></span>|<span data-ttu-id="34349-123">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="34349-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="34349-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="34349-124">Relationships</span></span>
<span data-ttu-id="34349-125">なし</span><span class="sxs-lookup"><span data-stu-id="34349-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="34349-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="34349-126">JSON Representation</span></span>
<span data-ttu-id="34349-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="34349-127">Here is a JSON representation of the resource.</span></span>
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





