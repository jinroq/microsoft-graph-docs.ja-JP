---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
author: tfitzmac
ms.openlocfilehash: 825e88dd5bd32cadfd9a8bfa291ab67036c8180b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343227"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="65df1-103">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65df1-103">appListItem resource type</span></span>

> <span data-ttu-id="65df1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="65df1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65df1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65df1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65df1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="65df1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65df1-107">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="65df1-107">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="65df1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65df1-108">Properties</span></span>
|<span data-ttu-id="65df1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65df1-109">Property</span></span>|<span data-ttu-id="65df1-110">種類</span><span class="sxs-lookup"><span data-stu-id="65df1-110">Type</span></span>|<span data-ttu-id="65df1-111">説明</span><span class="sxs-lookup"><span data-stu-id="65df1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65df1-112">名前</span><span class="sxs-lookup"><span data-stu-id="65df1-112">name</span></span>|<span data-ttu-id="65df1-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="65df1-113">String</span></span>|<span data-ttu-id="65df1-114">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="65df1-114">The application name</span></span>|
|<span data-ttu-id="65df1-115">発行元</span><span class="sxs-lookup"><span data-stu-id="65df1-115">publisher</span></span>|<span data-ttu-id="65df1-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="65df1-116">String</span></span>|<span data-ttu-id="65df1-117">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="65df1-117">The publisher of the application</span></span>|
|<span data-ttu-id="65df1-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="65df1-118">appStoreUrl</span></span>|<span data-ttu-id="65df1-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="65df1-119">String</span></span>|<span data-ttu-id="65df1-120">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="65df1-120">The Store URL of the application</span></span>|
|<span data-ttu-id="65df1-121">appId</span><span class="sxs-lookup"><span data-stu-id="65df1-121">appId</span></span>|<span data-ttu-id="65df1-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="65df1-122">String</span></span>|<span data-ttu-id="65df1-123">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="65df1-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="65df1-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="65df1-124">Relationships</span></span>
<span data-ttu-id="65df1-125">なし</span><span class="sxs-lookup"><span data-stu-id="65df1-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="65df1-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65df1-126">JSON Representation</span></span>
<span data-ttu-id="65df1-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65df1-127">Here is a JSON representation of the resource.</span></span>
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





