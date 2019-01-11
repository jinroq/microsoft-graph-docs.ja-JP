---
title: educationCsvDataProvider リソースの種類
description: 'CSV ファイルは、入力ソースとは、学校のデータの同期プロファイルを設定するために使用します。  '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: cb4d08a2a6750310a825f66ecfb0017abacd36fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878570"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="1d865-103">educationCsvDataProvider リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d865-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="1d865-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d865-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d865-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d865-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d865-106">CSV ファイルは、入力ソースとは、学校のデータの同期プロファイルを設定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="1d865-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="1d865-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="1d865-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1d865-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d865-108">Properties</span></span>

| <span data-ttu-id="1d865-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d865-109">Property</span></span> | <span data-ttu-id="1d865-110">種類</span><span class="sxs-lookup"><span data-stu-id="1d865-110">Type</span></span> | <span data-ttu-id="1d865-111">説明</span><span class="sxs-lookup"><span data-stu-id="1d865-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="1d865-112">**カスタマイズ**</span><span class="sxs-lookup"><span data-stu-id="1d865-112">**customizations**</span></span> | [<span data-ttu-id="1d865-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="1d865-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="1d865-114">同期プロファイルを適用するオプションのカスタマイズです。</span><span class="sxs-lookup"><span data-stu-id="1d865-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d865-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d865-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
