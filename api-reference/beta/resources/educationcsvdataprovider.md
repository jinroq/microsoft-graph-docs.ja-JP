---
title: educationCsvDataProvider リソースの種類
description: 'CSV ファイルは、入力ソースとは、学校のデータの同期プロファイルを設定するために使用します。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c9211d5f7ca25b78c6e76c3744f6941e3b172bb3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399347"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="c680c-103">educationCsvDataProvider リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c680c-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="c680c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c680c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c680c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c680c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c680c-106">CSV ファイルは、入力ソースとは、学校のデータの同期プロファイルを設定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="c680c-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="c680c-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="c680c-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c680c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c680c-108">Properties</span></span>

| <span data-ttu-id="c680c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c680c-109">Property</span></span> | <span data-ttu-id="c680c-110">型</span><span class="sxs-lookup"><span data-stu-id="c680c-110">Type</span></span> | <span data-ttu-id="c680c-111">説明</span><span class="sxs-lookup"><span data-stu-id="c680c-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c680c-112">**カスタマイズ**</span><span class="sxs-lookup"><span data-stu-id="c680c-112">**customizations**</span></span> | [<span data-ttu-id="c680c-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="c680c-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="c680c-114">同期プロファイルを適用するオプションのカスタマイズです。</span><span class="sxs-lookup"><span data-stu-id="c680c-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c680c-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c680c-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
