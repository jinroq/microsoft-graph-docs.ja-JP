---
title: windowsInformationProtectionDataRecoveryCertificate リソースの種類
description: Windows 情報保護の DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5e686ab1a6c1e586c8bd32c56d3480102503b4be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976255"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="9acab-103">windowsInformationProtectionDataRecoveryCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9acab-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="9acab-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9acab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9acab-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9acab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9acab-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9acab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9acab-107">Windows 情報保護の DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="9acab-107">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="9acab-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9acab-108">Properties</span></span>
|<span data-ttu-id="9acab-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9acab-109">Property</span></span>|<span data-ttu-id="9acab-110">種類</span><span class="sxs-lookup"><span data-stu-id="9acab-110">Type</span></span>|<span data-ttu-id="9acab-111">説明</span><span class="sxs-lookup"><span data-stu-id="9acab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9acab-112">subjectName</span><span class="sxs-lookup"><span data-stu-id="9acab-112">subjectName</span></span>|<span data-ttu-id="9acab-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9acab-113">String</span></span>|<span data-ttu-id="9acab-114">データ回復証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="9acab-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="9acab-115">説明</span><span class="sxs-lookup"><span data-stu-id="9acab-115">description</span></span>|<span data-ttu-id="9acab-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9acab-116">String</span></span>|<span data-ttu-id="9acab-117">データ回復証明書の説明</span><span class="sxs-lookup"><span data-stu-id="9acab-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="9acab-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9acab-118">expirationDateTime</span></span>|<span data-ttu-id="9acab-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9acab-119">DateTimeOffset</span></span>|<span data-ttu-id="9acab-120">データ回復証明書の有効期限日時</span><span class="sxs-lookup"><span data-stu-id="9acab-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="9acab-121">certificate</span><span class="sxs-lookup"><span data-stu-id="9acab-121">certificate</span></span>|<span data-ttu-id="9acab-122">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="9acab-122">Binary</span></span>|<span data-ttu-id="9acab-123">データ回復証明書</span><span class="sxs-lookup"><span data-stu-id="9acab-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="9acab-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9acab-124">Relationships</span></span>
<span data-ttu-id="9acab-125">なし</span><span class="sxs-lookup"><span data-stu-id="9acab-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9acab-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9acab-126">JSON Representation</span></span>
<span data-ttu-id="9acab-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9acab-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```





