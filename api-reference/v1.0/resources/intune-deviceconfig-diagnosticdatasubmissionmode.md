---
title: diagnosticDataSubmissionMode 列挙型
description: デバイスが診断データと使用統計情報 (Watson など) を送信できるようにします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c0707b97e60da406210d6a091ed0dd4efaa2299
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578023"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="92889-103">diagnosticDataSubmissionMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="92889-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="92889-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92889-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92889-105">デバイスが診断データと使用統計情報 (Watson など) を送信できるようにします。</span><span class="sxs-lookup"><span data-stu-id="92889-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="92889-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="92889-106">Members</span></span>
|<span data-ttu-id="92889-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="92889-107">Member</span></span>|<span data-ttu-id="92889-108">値</span><span class="sxs-lookup"><span data-stu-id="92889-108">Value</span></span>|<span data-ttu-id="92889-109">説明</span><span class="sxs-lookup"><span data-stu-id="92889-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92889-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="92889-110">userDefined</span></span>|<span data-ttu-id="92889-111">.0</span><span class="sxs-lookup"><span data-stu-id="92889-111">0</span></span>|<span data-ttu-id="92889-112">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="92889-112">Allow the user to set.</span></span>|
|<span data-ttu-id="92889-113">なし</span><span class="sxs-lookup"><span data-stu-id="92889-113">none</span></span>|<span data-ttu-id="92889-114">1 </span><span class="sxs-lookup"><span data-stu-id="92889-114">1</span></span>|<span data-ttu-id="92889-115">テレメトリデータは、OS コンポーネントから送信されません。</span><span class="sxs-lookup"><span data-stu-id="92889-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="92889-116">注: この値は、エンタープライズおよびサーバーデバイスにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="92889-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="92889-117">他のデバイスでこの設定を使用することは、値を1に設定するのと同じです。</span><span class="sxs-lookup"><span data-stu-id="92889-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="92889-118">基本的な</span><span class="sxs-lookup"><span data-stu-id="92889-118">basic</span></span>|<span data-ttu-id="92889-119">2 </span><span class="sxs-lookup"><span data-stu-id="92889-119">2</span></span>|<span data-ttu-id="92889-120">基本的なテレメトリデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="92889-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="92889-121">保護</span><span class="sxs-lookup"><span data-stu-id="92889-121">enhanced</span></span>|<span data-ttu-id="92889-122">3 </span><span class="sxs-lookup"><span data-stu-id="92889-122">3</span></span>|<span data-ttu-id="92889-123">利用状況データおよびインサイトデータを含む、拡張されたテレメトリデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="92889-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="92889-124">完全</span><span class="sxs-lookup"><span data-stu-id="92889-124">full</span></span>|<span data-ttu-id="92889-125">4 </span><span class="sxs-lookup"><span data-stu-id="92889-125">4</span></span>|<span data-ttu-id="92889-126">システム状態などの診断データを含む完全なテレメトリデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="92889-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



