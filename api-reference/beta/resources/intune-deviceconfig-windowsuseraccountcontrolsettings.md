---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザーアカウント制御設定に指定できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b63fe44abfb0a06e5978d78e49c392c08122e38
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795787"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="8c50f-103">windowsUserAccountControlSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="8c50f-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="8c50f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c50f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c50f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8c50f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c50f-106">Windows ユーザーアカウント制御設定に指定できる値。</span><span class="sxs-lookup"><span data-stu-id="8c50f-106">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="8c50f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="8c50f-107">Members</span></span>
|<span data-ttu-id="8c50f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8c50f-108">Member</span></span>|<span data-ttu-id="8c50f-109">値</span><span class="sxs-lookup"><span data-stu-id="8c50f-109">Value</span></span>|<span data-ttu-id="8c50f-110">説明</span><span class="sxs-lookup"><span data-stu-id="8c50f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c50f-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="8c50f-111">userDefined</span></span>|<span data-ttu-id="8c50f-112">.0</span><span class="sxs-lookup"><span data-stu-id="8c50f-112">0</span></span>|<span data-ttu-id="8c50f-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="8c50f-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="8c50f-114">常に通知</span><span class="sxs-lookup"><span data-stu-id="8c50f-114">alwaysNotify</span></span>|<span data-ttu-id="8c50f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="8c50f-115">1</span></span>|<span data-ttu-id="8c50f-116">常に通知します。</span><span class="sxs-lookup"><span data-stu-id="8c50f-116">Always notify.</span></span>|
|<span data-ttu-id="8c50f-117">notifyonappchanges</span><span class="sxs-lookup"><span data-stu-id="8c50f-117">notifyOnAppChanges</span></span>|<span data-ttu-id="8c50f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="8c50f-118">2</span></span>|<span data-ttu-id="8c50f-119">アプリの変更について通知します。</span><span class="sxs-lookup"><span data-stu-id="8c50f-119">Notify on app changes.</span></span>|
|<span data-ttu-id="8c50f-120">notifyonappのすべての非追加暗転</span><span class="sxs-lookup"><span data-stu-id="8c50f-120">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="8c50f-121">1/3</span><span class="sxs-lookup"><span data-stu-id="8c50f-121">3</span></span>|<span data-ttu-id="8c50f-122">デスクトップを暗転せずに、アプリの変更について通知します。</span><span class="sxs-lookup"><span data-stu-id="8c50f-122">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="8c50f-123">neverNotify</span><span class="sxs-lookup"><span data-stu-id="8c50f-123">neverNotify</span></span>|<span data-ttu-id="8c50f-124">2/4</span><span class="sxs-lookup"><span data-stu-id="8c50f-124">4</span></span>|<span data-ttu-id="8c50f-125">通知しません。</span><span class="sxs-lookup"><span data-stu-id="8c50f-125">Never notify.</span></span>|





