---
title: windowsInformationProtectionDataRecoveryCertificate リソースの種類
description: Windows 情報保護の DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2a40fc3ab500fe6aa2a5b0f373c78524444b5bd1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971859"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="4ce36-103">windowsInformationProtectionDataRecoveryCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4ce36-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="4ce36-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4ce36-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ce36-105">Windows 情報保護の DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="4ce36-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="4ce36-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ce36-106">Properties</span></span>
|<span data-ttu-id="4ce36-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ce36-107">Property</span></span>|<span data-ttu-id="4ce36-108">種類</span><span class="sxs-lookup"><span data-stu-id="4ce36-108">Type</span></span>|<span data-ttu-id="4ce36-109">説明</span><span class="sxs-lookup"><span data-stu-id="4ce36-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ce36-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="4ce36-110">subjectName</span></span>|<span data-ttu-id="4ce36-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4ce36-111">String</span></span>|<span data-ttu-id="4ce36-112">データ回復証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="4ce36-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="4ce36-113">説明</span><span class="sxs-lookup"><span data-stu-id="4ce36-113">description</span></span>|<span data-ttu-id="4ce36-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4ce36-114">String</span></span>|<span data-ttu-id="4ce36-115">データ回復証明書の説明</span><span class="sxs-lookup"><span data-stu-id="4ce36-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="4ce36-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4ce36-116">expirationDateTime</span></span>|<span data-ttu-id="4ce36-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ce36-117">DateTimeOffset</span></span>|<span data-ttu-id="4ce36-118">データ回復証明書の有効期限日時</span><span class="sxs-lookup"><span data-stu-id="4ce36-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="4ce36-119">certificate</span><span class="sxs-lookup"><span data-stu-id="4ce36-119">certificate</span></span>|<span data-ttu-id="4ce36-120">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="4ce36-120">Binary</span></span>|<span data-ttu-id="4ce36-121">データ回復証明書</span><span class="sxs-lookup"><span data-stu-id="4ce36-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ce36-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4ce36-122">Relationships</span></span>
<span data-ttu-id="4ce36-123">なし</span><span class="sxs-lookup"><span data-stu-id="4ce36-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4ce36-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4ce36-124">JSON Representation</span></span>
<span data-ttu-id="4ce36-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4ce36-125">Here is a JSON representation of the resource.</span></span>
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



