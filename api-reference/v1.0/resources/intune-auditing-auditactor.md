---
title: auditActor リソースの種類
description: 監査アクターのプロパティが含まれるクラス。
author: tfitzmac
ms.openlocfilehash: de2fc78bcc02565da102beb57c077646effc443b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325019"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="be057-103">auditActor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be057-103">auditActor resource type</span></span>

> <span data-ttu-id="be057-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="be057-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be057-105">監査アクターのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="be057-105">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="be057-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be057-106">Properties</span></span>
|<span data-ttu-id="be057-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be057-107">Property</span></span>|<span data-ttu-id="be057-108">種類</span><span class="sxs-lookup"><span data-stu-id="be057-108">Type</span></span>|<span data-ttu-id="be057-109">説明</span><span class="sxs-lookup"><span data-stu-id="be057-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be057-110">type</span><span class="sxs-lookup"><span data-stu-id="be057-110">type</span></span>|<span data-ttu-id="be057-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="be057-111">String</span></span>|<span data-ttu-id="be057-112">アクターの種類。</span><span class="sxs-lookup"><span data-stu-id="be057-112">Actor Type.</span></span>|
|<span data-ttu-id="be057-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="be057-113">userPermissions</span></span>|<span data-ttu-id="be057-114">String コレクション</span><span class="sxs-lookup"><span data-stu-id="be057-114">String collection</span></span>|<span data-ttu-id="be057-115">監査の実行時におけるユーザーのアクセス許可の一覧。</span><span class="sxs-lookup"><span data-stu-id="be057-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="be057-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="be057-116">applicationId</span></span>|<span data-ttu-id="be057-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="be057-117">String</span></span>|<span data-ttu-id="be057-118">AAD アプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="be057-118">AAD Application Id.</span></span>|
|<span data-ttu-id="be057-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="be057-119">applicationDisplayName</span></span>|<span data-ttu-id="be057-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="be057-120">String</span></span>|<span data-ttu-id="be057-121">アプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="be057-121">Name of the Application.</span></span>|
|<span data-ttu-id="be057-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="be057-122">userPrincipalName</span></span>|<span data-ttu-id="be057-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="be057-123">String</span></span>|<span data-ttu-id="be057-124">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="be057-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="be057-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="be057-125">servicePrincipalName</span></span>|<span data-ttu-id="be057-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="be057-126">String</span></span>|<span data-ttu-id="be057-127">サービス プリンシパル名 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="be057-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="be057-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="be057-128">ipAddress</span></span>|<span data-ttu-id="be057-129">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="be057-129">String</span></span>|<span data-ttu-id="be057-130">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="be057-130">IPAddress.</span></span>|
|<span data-ttu-id="be057-131">userId</span><span class="sxs-lookup"><span data-stu-id="be057-131">userId</span></span>|<span data-ttu-id="be057-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="be057-132">String</span></span>|<span data-ttu-id="be057-133">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="be057-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be057-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="be057-134">Relationships</span></span>
<span data-ttu-id="be057-135">なし</span><span class="sxs-lookup"><span data-stu-id="be057-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="be057-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be057-136">JSON Representation</span></span>
<span data-ttu-id="be057-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="be057-137">Here is a JSON representation of the resource.</span></span>
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



