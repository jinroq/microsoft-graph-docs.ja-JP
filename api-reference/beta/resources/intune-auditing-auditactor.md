---
title: auditActor リソースの種類
description: 監査アクターのプロパティが含まれるクラス。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 633f5f4c513d6f770df643c26934b994a134e450
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985620"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="34665-103">auditActor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="34665-103">auditActor resource type</span></span>

> <span data-ttu-id="34665-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34665-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34665-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="34665-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34665-106">監査アクターのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="34665-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="34665-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34665-107">Properties</span></span>
|<span data-ttu-id="34665-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34665-108">Property</span></span>|<span data-ttu-id="34665-109">型</span><span class="sxs-lookup"><span data-stu-id="34665-109">Type</span></span>|<span data-ttu-id="34665-110">説明</span><span class="sxs-lookup"><span data-stu-id="34665-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34665-111">type</span><span class="sxs-lookup"><span data-stu-id="34665-111">type</span></span>|<span data-ttu-id="34665-112">String</span><span class="sxs-lookup"><span data-stu-id="34665-112">String</span></span>|<span data-ttu-id="34665-113">アクターの種類。</span><span class="sxs-lookup"><span data-stu-id="34665-113">Actor Type.</span></span>|
|<span data-ttu-id="34665-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="34665-114">userPermissions</span></span>|<span data-ttu-id="34665-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="34665-115">String collection</span></span>|<span data-ttu-id="34665-116">監査の実行時におけるユーザーのアクセス許可の一覧。</span><span class="sxs-lookup"><span data-stu-id="34665-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="34665-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="34665-117">applicationId</span></span>|<span data-ttu-id="34665-118">String</span><span class="sxs-lookup"><span data-stu-id="34665-118">String</span></span>|<span data-ttu-id="34665-119">AAD アプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="34665-119">AAD Application Id.</span></span>|
|<span data-ttu-id="34665-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="34665-120">applicationDisplayName</span></span>|<span data-ttu-id="34665-121">String</span><span class="sxs-lookup"><span data-stu-id="34665-121">String</span></span>|<span data-ttu-id="34665-122">アプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="34665-122">Name of the Application.</span></span>|
|<span data-ttu-id="34665-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="34665-123">userPrincipalName</span></span>|<span data-ttu-id="34665-124">文字列</span><span class="sxs-lookup"><span data-stu-id="34665-124">String</span></span>|<span data-ttu-id="34665-125">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="34665-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="34665-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="34665-126">servicePrincipalName</span></span>|<span data-ttu-id="34665-127">String</span><span class="sxs-lookup"><span data-stu-id="34665-127">String</span></span>|<span data-ttu-id="34665-128">サービス プリンシパル名 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="34665-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="34665-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="34665-129">ipAddress</span></span>|<span data-ttu-id="34665-130">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="34665-130">String</span></span>|<span data-ttu-id="34665-131">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="34665-131">IPAddress.</span></span>|
|<span data-ttu-id="34665-132">userId</span><span class="sxs-lookup"><span data-stu-id="34665-132">userId</span></span>|<span data-ttu-id="34665-133">String</span><span class="sxs-lookup"><span data-stu-id="34665-133">String</span></span>|<span data-ttu-id="34665-134">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="34665-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34665-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="34665-135">Relationships</span></span>
<span data-ttu-id="34665-136">なし</span><span class="sxs-lookup"><span data-stu-id="34665-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34665-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="34665-137">JSON Representation</span></span>
<span data-ttu-id="34665-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="34665-138">Here is a JSON representation of the resource.</span></span>
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





