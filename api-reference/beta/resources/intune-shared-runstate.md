---
title: runState 列挙型
description: デバイス管理スクリプトの実行状態の種類を示します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d77f3ef9a2d7fd37edeaf2b4cc25d5e6d5bfcf4f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347851"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="9845d-103">runState 列挙型</span><span class="sxs-lookup"><span data-stu-id="9845d-103">runState enum type</span></span>

> <span data-ttu-id="9845d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9845d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9845d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9845d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9845d-106">デバイス管理スクリプトの実行状態の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="9845d-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="9845d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9845d-107">Members</span></span>
|<span data-ttu-id="9845d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9845d-108">Member</span></span>|<span data-ttu-id="9845d-109">値</span><span class="sxs-lookup"><span data-stu-id="9845d-109">Value</span></span>|<span data-ttu-id="9845d-110">説明</span><span class="sxs-lookup"><span data-stu-id="9845d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9845d-111">不明</span><span class="sxs-lookup"><span data-stu-id="9845d-111">unknown</span></span>|<span data-ttu-id="9845d-112">.0</span><span class="sxs-lookup"><span data-stu-id="9845d-112">0</span></span>|<span data-ttu-id="9845d-113">不明な結果です。</span><span class="sxs-lookup"><span data-stu-id="9845d-113">Unknown result.</span></span>|
|<span data-ttu-id="9845d-114">success</span><span class="sxs-lookup"><span data-stu-id="9845d-114">success</span></span>|<span data-ttu-id="9845d-115">1-d</span><span class="sxs-lookup"><span data-stu-id="9845d-115">1</span></span>|<span data-ttu-id="9845d-116">スクリプトは正常に実行されます。</span><span class="sxs-lookup"><span data-stu-id="9845d-116">Script is run successfully.</span></span>|
|<span data-ttu-id="9845d-117">fail</span><span class="sxs-lookup"><span data-stu-id="9845d-117">fail</span></span>|<span data-ttu-id="9845d-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="9845d-118">2</span></span>|<span data-ttu-id="9845d-119">スクリプトの実行に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="9845d-119">Script failed to run.</span></span>|
|<span data-ttu-id="9845d-120">error</span><span class="sxs-lookup"><span data-stu-id="9845d-120">error</span></span>|<span data-ttu-id="9845d-121">1/3</span><span class="sxs-lookup"><span data-stu-id="9845d-121">3</span></span>|<span data-ttu-id="9845d-122">検出スクリプトヒットエラー。</span><span class="sxs-lookup"><span data-stu-id="9845d-122">Discovery script hits error.</span></span>|
|<span data-ttu-id="9845d-123">対する</span><span class="sxs-lookup"><span data-stu-id="9845d-123">pending</span></span>|<span data-ttu-id="9845d-124">2/4</span><span class="sxs-lookup"><span data-stu-id="9845d-124">4</span></span>|<span data-ttu-id="9845d-125">スクリプトの実行が保留中です。</span><span class="sxs-lookup"><span data-stu-id="9845d-125">Script is pending to execute.</span></span>|



