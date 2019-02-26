---
title: diagnosticDataSubmissionMode 列挙型
description: デバイスが診断データと使用統計情報 (Watson など) を送信できるようにします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c0707b97e60da406210d6a091ed0dd4efaa2299
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251035"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="b7738-103">diagnosticDataSubmissionMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="b7738-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="b7738-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b7738-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7738-105">デバイスが診断データと使用統計情報 (Watson など) を送信できるようにします。</span><span class="sxs-lookup"><span data-stu-id="b7738-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="b7738-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="b7738-106">Members</span></span>
|<span data-ttu-id="b7738-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b7738-107">Member</span></span>|<span data-ttu-id="b7738-108">値</span><span class="sxs-lookup"><span data-stu-id="b7738-108">Value</span></span>|<span data-ttu-id="b7738-109">説明</span><span class="sxs-lookup"><span data-stu-id="b7738-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7738-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="b7738-110">userDefined</span></span>|<span data-ttu-id="b7738-111">.0</span><span class="sxs-lookup"><span data-stu-id="b7738-111">0</span></span>|<span data-ttu-id="b7738-112">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="b7738-112">Allow the user to set.</span></span>|
|<span data-ttu-id="b7738-113">none</span><span class="sxs-lookup"><span data-stu-id="b7738-113">none</span></span>|<span data-ttu-id="b7738-114">1-d</span><span class="sxs-lookup"><span data-stu-id="b7738-114">1</span></span>|<span data-ttu-id="b7738-115">テレメトリデータは、OS コンポーネントから送信されません。</span><span class="sxs-lookup"><span data-stu-id="b7738-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="b7738-116">注: この値は、エンタープライズおよびサーバーデバイスにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="b7738-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="b7738-117">他のデバイスでこの設定を使用することは、値を1に設定するのと同じです。</span><span class="sxs-lookup"><span data-stu-id="b7738-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="b7738-118">基本的な</span><span class="sxs-lookup"><span data-stu-id="b7738-118">basic</span></span>|<span data-ttu-id="b7738-119">pbm-2</span><span class="sxs-lookup"><span data-stu-id="b7738-119">2</span></span>|<span data-ttu-id="b7738-120">基本的なテレメトリデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="b7738-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="b7738-121">保護</span><span class="sxs-lookup"><span data-stu-id="b7738-121">enhanced</span></span>|<span data-ttu-id="b7738-122">1/3</span><span class="sxs-lookup"><span data-stu-id="b7738-122">3</span></span>|<span data-ttu-id="b7738-123">利用状況データおよびインサイトデータを含む、拡張されたテレメトリデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="b7738-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="b7738-124">完全</span><span class="sxs-lookup"><span data-stu-id="b7738-124">full</span></span>|<span data-ttu-id="b7738-125">2/4</span><span class="sxs-lookup"><span data-stu-id="b7738-125">4</span></span>|<span data-ttu-id="b7738-126">システム状態などの診断データを含む完全なテレメトリデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="b7738-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



