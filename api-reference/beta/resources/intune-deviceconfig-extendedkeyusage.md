---
title: extendedkeyusage リソースの種類
description: カスタム拡張キー使用法の定義
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1487d217693135e26df99d4d72491abac4123ba7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173291"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="65159-103">extendedkeyusage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65159-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="65159-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65159-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65159-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="65159-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65159-106">カスタム拡張キー使用法の定義</span><span class="sxs-lookup"><span data-stu-id="65159-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="65159-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65159-107">Properties</span></span>
|<span data-ttu-id="65159-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65159-108">Property</span></span>|<span data-ttu-id="65159-109">型</span><span class="sxs-lookup"><span data-stu-id="65159-109">Type</span></span>|<span data-ttu-id="65159-110">説明</span><span class="sxs-lookup"><span data-stu-id="65159-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65159-111">name</span><span class="sxs-lookup"><span data-stu-id="65159-111">name</span></span>|<span data-ttu-id="65159-112">String</span><span class="sxs-lookup"><span data-stu-id="65159-112">String</span></span>|<span data-ttu-id="65159-113">拡張キー使用法の名前</span><span class="sxs-lookup"><span data-stu-id="65159-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="65159-114">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="65159-114">objectIdentifier</span></span>|<span data-ttu-id="65159-115">String</span><span class="sxs-lookup"><span data-stu-id="65159-115">String</span></span>|<span data-ttu-id="65159-116">拡張キー使用法のオブジェクト識別子</span><span class="sxs-lookup"><span data-stu-id="65159-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="65159-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="65159-117">Relationships</span></span>
<span data-ttu-id="65159-118">なし</span><span class="sxs-lookup"><span data-stu-id="65159-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65159-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65159-119">JSON Representation</span></span>
<span data-ttu-id="65159-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65159-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```




