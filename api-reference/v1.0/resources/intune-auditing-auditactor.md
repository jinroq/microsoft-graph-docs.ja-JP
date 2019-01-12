---
title: auditActor リソースの種類
description: 監査アクターのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ba63fd04d917a464933e749622a5abf959c2859e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948703"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="dcb40-103">auditActor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dcb40-103">auditActor resource type</span></span>

> <span data-ttu-id="dcb40-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dcb40-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dcb40-105">監査アクターのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="dcb40-105">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="dcb40-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcb40-106">Properties</span></span>
|<span data-ttu-id="dcb40-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcb40-107">Property</span></span>|<span data-ttu-id="dcb40-108">種類</span><span class="sxs-lookup"><span data-stu-id="dcb40-108">Type</span></span>|<span data-ttu-id="dcb40-109">説明</span><span class="sxs-lookup"><span data-stu-id="dcb40-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcb40-110">type</span><span class="sxs-lookup"><span data-stu-id="dcb40-110">type</span></span>|<span data-ttu-id="dcb40-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dcb40-111">String</span></span>|<span data-ttu-id="dcb40-112">アクターの種類。</span><span class="sxs-lookup"><span data-stu-id="dcb40-112">Actor Type.</span></span>|
|<span data-ttu-id="dcb40-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="dcb40-113">userPermissions</span></span>|<span data-ttu-id="dcb40-114">String コレクション</span><span class="sxs-lookup"><span data-stu-id="dcb40-114">String collection</span></span>|<span data-ttu-id="dcb40-115">監査の実行時におけるユーザーのアクセス許可の一覧。</span><span class="sxs-lookup"><span data-stu-id="dcb40-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="dcb40-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="dcb40-116">applicationId</span></span>|<span data-ttu-id="dcb40-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dcb40-117">String</span></span>|<span data-ttu-id="dcb40-118">AAD アプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="dcb40-118">AAD Application Id.</span></span>|
|<span data-ttu-id="dcb40-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="dcb40-119">applicationDisplayName</span></span>|<span data-ttu-id="dcb40-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dcb40-120">String</span></span>|<span data-ttu-id="dcb40-121">アプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="dcb40-121">Name of the Application.</span></span>|
|<span data-ttu-id="dcb40-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dcb40-122">userPrincipalName</span></span>|<span data-ttu-id="dcb40-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dcb40-123">String</span></span>|<span data-ttu-id="dcb40-124">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="dcb40-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="dcb40-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="dcb40-125">servicePrincipalName</span></span>|<span data-ttu-id="dcb40-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dcb40-126">String</span></span>|<span data-ttu-id="dcb40-127">サービス プリンシパル名 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="dcb40-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="dcb40-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="dcb40-128">ipAddress</span></span>|<span data-ttu-id="dcb40-129">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dcb40-129">String</span></span>|<span data-ttu-id="dcb40-130">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="dcb40-130">IPAddress.</span></span>|
|<span data-ttu-id="dcb40-131">userId</span><span class="sxs-lookup"><span data-stu-id="dcb40-131">userId</span></span>|<span data-ttu-id="dcb40-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dcb40-132">String</span></span>|<span data-ttu-id="dcb40-133">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="dcb40-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcb40-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dcb40-134">Relationships</span></span>
<span data-ttu-id="dcb40-135">なし</span><span class="sxs-lookup"><span data-stu-id="dcb40-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dcb40-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dcb40-136">JSON Representation</span></span>
<span data-ttu-id="dcb40-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dcb40-137">Here is a JSON representation of the resource.</span></span>
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



