---
title: customSubjectAlternativeName リソースの種類
description: カスタムのサブジェクトの別名定義
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 069cc1f6d93c785e4fc774d7988e0fc80febbb12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954121"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="bd33c-103">customSubjectAlternativeName リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bd33c-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="bd33c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bd33c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd33c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd33c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd33c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bd33c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd33c-107">カスタムのサブジェクトの別名定義</span><span class="sxs-lookup"><span data-stu-id="bd33c-107">Custom Subject Alternative Name definition</span></span>
## <a name="properties"></a><span data-ttu-id="bd33c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd33c-108">Properties</span></span>
|<span data-ttu-id="bd33c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd33c-109">Property</span></span>|<span data-ttu-id="bd33c-110">種類</span><span class="sxs-lookup"><span data-stu-id="bd33c-110">Type</span></span>|<span data-ttu-id="bd33c-111">説明</span><span class="sxs-lookup"><span data-stu-id="bd33c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd33c-112">sanType</span><span class="sxs-lookup"><span data-stu-id="bd33c-112">sanType</span></span>|[<span data-ttu-id="bd33c-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bd33c-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="bd33c-114">SAN のカスタム型です。</span><span class="sxs-lookup"><span data-stu-id="bd33c-114">Custom SAN Type.</span></span> <span data-ttu-id="bd33c-115">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="bd33c-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="bd33c-116">名前</span><span class="sxs-lookup"><span data-stu-id="bd33c-116">name</span></span>|<span data-ttu-id="bd33c-117">String</span><span class="sxs-lookup"><span data-stu-id="bd33c-117">String</span></span>|<span data-ttu-id="bd33c-118">SAN のカスタム名</span><span class="sxs-lookup"><span data-stu-id="bd33c-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd33c-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bd33c-119">Relationships</span></span>
<span data-ttu-id="bd33c-120">なし</span><span class="sxs-lookup"><span data-stu-id="bd33c-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bd33c-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bd33c-121">JSON Representation</span></span>
<span data-ttu-id="bd33c-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bd33c-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```





