---
title: auditActor リソースの種類
description: 監査アクターのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 14b4ce53d46897a84da8fab468ba2ad6aa99b30e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820049"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="4b1b8-103">auditActor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b1b8-103">auditActor resource type</span></span>

> <span data-ttu-id="4b1b8-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4b1b8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b1b8-105">監査アクターのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="4b1b8-105">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="4b1b8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b1b8-106">Properties</span></span>
|<span data-ttu-id="4b1b8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b1b8-107">Property</span></span>|<span data-ttu-id="4b1b8-108">種類</span><span class="sxs-lookup"><span data-stu-id="4b1b8-108">Type</span></span>|<span data-ttu-id="4b1b8-109">説明</span><span class="sxs-lookup"><span data-stu-id="4b1b8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b1b8-110">type</span><span class="sxs-lookup"><span data-stu-id="4b1b8-110">type</span></span>|<span data-ttu-id="4b1b8-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4b1b8-111">String</span></span>|<span data-ttu-id="4b1b8-112">アクターの種類。</span><span class="sxs-lookup"><span data-stu-id="4b1b8-112">Actor Type.</span></span>|
|<span data-ttu-id="4b1b8-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="4b1b8-113">userPermissions</span></span>|<span data-ttu-id="4b1b8-114">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4b1b8-114">String collection</span></span>|<span data-ttu-id="4b1b8-115">監査の実行時におけるユーザーのアクセス許可の一覧。</span><span class="sxs-lookup"><span data-stu-id="4b1b8-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="4b1b8-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="4b1b8-116">applicationId</span></span>|<span data-ttu-id="4b1b8-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4b1b8-117">String</span></span>|<span data-ttu-id="4b1b8-118">AAD アプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="4b1b8-118">AAD Application Id.</span></span>|
|<span data-ttu-id="4b1b8-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="4b1b8-119">applicationDisplayName</span></span>|<span data-ttu-id="4b1b8-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4b1b8-120">String</span></span>|<span data-ttu-id="4b1b8-121">アプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="4b1b8-121">Name of the Application.</span></span>|
|<span data-ttu-id="4b1b8-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4b1b8-122">userPrincipalName</span></span>|<span data-ttu-id="4b1b8-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4b1b8-123">String</span></span>|<span data-ttu-id="4b1b8-124">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="4b1b8-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="4b1b8-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="4b1b8-125">servicePrincipalName</span></span>|<span data-ttu-id="4b1b8-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4b1b8-126">String</span></span>|<span data-ttu-id="4b1b8-127">サービス プリンシパル名 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="4b1b8-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="4b1b8-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="4b1b8-128">ipAddress</span></span>|<span data-ttu-id="4b1b8-129">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4b1b8-129">String</span></span>|<span data-ttu-id="4b1b8-130">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="4b1b8-130">IPAddress.</span></span>|
|<span data-ttu-id="4b1b8-131">userId</span><span class="sxs-lookup"><span data-stu-id="4b1b8-131">userId</span></span>|<span data-ttu-id="4b1b8-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4b1b8-132">String</span></span>|<span data-ttu-id="4b1b8-133">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="4b1b8-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b1b8-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4b1b8-134">Relationships</span></span>
<span data-ttu-id="4b1b8-135">なし</span><span class="sxs-lookup"><span data-stu-id="4b1b8-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b1b8-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b1b8-136">JSON Representation</span></span>
<span data-ttu-id="4b1b8-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4b1b8-137">Here is a JSON representation of the resource.</span></span>
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



