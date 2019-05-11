---
title: diagnosticDataSubmissionMode 列挙型
description: デバイスが診断データと使用統計情報 (Watson など) を送信できるようにします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ba90c6cbbd8e242e4cd5902a938d5e670d7d2d7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946876"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="d9e12-103">diagnosticDataSubmissionMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="d9e12-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="d9e12-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9e12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9e12-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d9e12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9e12-106">デバイスが診断データと使用統計情報 (Watson など) を送信できるようにします。</span><span class="sxs-lookup"><span data-stu-id="d9e12-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="d9e12-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d9e12-107">Members</span></span>
|<span data-ttu-id="d9e12-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d9e12-108">Member</span></span>|<span data-ttu-id="d9e12-109">値</span><span class="sxs-lookup"><span data-stu-id="d9e12-109">Value</span></span>|<span data-ttu-id="d9e12-110">説明</span><span class="sxs-lookup"><span data-stu-id="d9e12-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9e12-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="d9e12-111">userDefined</span></span>|<span data-ttu-id="d9e12-112">.0</span><span class="sxs-lookup"><span data-stu-id="d9e12-112">0</span></span>|<span data-ttu-id="d9e12-113">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="d9e12-113">Allow the user to set.</span></span>|
|<span data-ttu-id="d9e12-114">none</span><span class="sxs-lookup"><span data-stu-id="d9e12-114">none</span></span>|<span data-ttu-id="d9e12-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d9e12-115">1</span></span>|<span data-ttu-id="d9e12-116">テレメトリデータは、OS コンポーネントから送信されません。</span><span class="sxs-lookup"><span data-stu-id="d9e12-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="d9e12-117">注: この値は、エンタープライズおよびサーバーデバイスにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="d9e12-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="d9e12-118">他のデバイスでこの設定を使用することは、値を1に設定するのと同じです。</span><span class="sxs-lookup"><span data-stu-id="d9e12-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="d9e12-119">基本的な</span><span class="sxs-lookup"><span data-stu-id="d9e12-119">basic</span></span>|<span data-ttu-id="d9e12-120">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d9e12-120">2</span></span>|<span data-ttu-id="d9e12-121">基本的なテレメトリデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="d9e12-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="d9e12-122">保護</span><span class="sxs-lookup"><span data-stu-id="d9e12-122">enhanced</span></span>|<span data-ttu-id="d9e12-123">1/3</span><span class="sxs-lookup"><span data-stu-id="d9e12-123">3</span></span>|<span data-ttu-id="d9e12-124">利用状況データおよびインサイトデータを含む、拡張されたテレメトリデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="d9e12-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="d9e12-125">完全</span><span class="sxs-lookup"><span data-stu-id="d9e12-125">full</span></span>|<span data-ttu-id="d9e12-126">2/4</span><span class="sxs-lookup"><span data-stu-id="d9e12-126">4</span></span>|<span data-ttu-id="d9e12-127">システム状態などの診断データを含む完全なテレメトリデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="d9e12-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




