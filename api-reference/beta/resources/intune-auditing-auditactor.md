---
title: auditActor リソースの種類
description: 監査アクターのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4c6dddd2863f881c026eb848c643bdc55cbbb372
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873914"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="74f72-103">auditActor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="74f72-103">auditActor resource type</span></span>

> <span data-ttu-id="74f72-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="74f72-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74f72-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74f72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74f72-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="74f72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74f72-107">監査アクターのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="74f72-107">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="74f72-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74f72-108">Properties</span></span>
|<span data-ttu-id="74f72-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74f72-109">Property</span></span>|<span data-ttu-id="74f72-110">種類</span><span class="sxs-lookup"><span data-stu-id="74f72-110">Type</span></span>|<span data-ttu-id="74f72-111">説明</span><span class="sxs-lookup"><span data-stu-id="74f72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74f72-112">type</span><span class="sxs-lookup"><span data-stu-id="74f72-112">type</span></span>|<span data-ttu-id="74f72-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="74f72-113">String</span></span>|<span data-ttu-id="74f72-114">アクターの種類。</span><span class="sxs-lookup"><span data-stu-id="74f72-114">Actor Type.</span></span>|
|<span data-ttu-id="74f72-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="74f72-115">userPermissions</span></span>|<span data-ttu-id="74f72-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="74f72-116">String collection</span></span>|<span data-ttu-id="74f72-117">監査の実行時におけるユーザーのアクセス許可の一覧。</span><span class="sxs-lookup"><span data-stu-id="74f72-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="74f72-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="74f72-118">applicationId</span></span>|<span data-ttu-id="74f72-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="74f72-119">String</span></span>|<span data-ttu-id="74f72-120">AAD アプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="74f72-120">AAD Application Id.</span></span>|
|<span data-ttu-id="74f72-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="74f72-121">applicationDisplayName</span></span>|<span data-ttu-id="74f72-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="74f72-122">String</span></span>|<span data-ttu-id="74f72-123">アプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="74f72-123">Name of the Application.</span></span>|
|<span data-ttu-id="74f72-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="74f72-124">userPrincipalName</span></span>|<span data-ttu-id="74f72-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="74f72-125">String</span></span>|<span data-ttu-id="74f72-126">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="74f72-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="74f72-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="74f72-127">servicePrincipalName</span></span>|<span data-ttu-id="74f72-128">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="74f72-128">String</span></span>|<span data-ttu-id="74f72-129">サービス プリンシパル名 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="74f72-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="74f72-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="74f72-130">ipAddress</span></span>|<span data-ttu-id="74f72-131">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="74f72-131">String</span></span>|<span data-ttu-id="74f72-132">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="74f72-132">IPAddress.</span></span>|
|<span data-ttu-id="74f72-133">userId</span><span class="sxs-lookup"><span data-stu-id="74f72-133">userId</span></span>|<span data-ttu-id="74f72-134">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="74f72-134">String</span></span>|<span data-ttu-id="74f72-135">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="74f72-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74f72-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="74f72-136">Relationships</span></span>
<span data-ttu-id="74f72-137">なし</span><span class="sxs-lookup"><span data-stu-id="74f72-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="74f72-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="74f72-138">JSON Representation</span></span>
<span data-ttu-id="74f72-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="74f72-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String"
}
```





