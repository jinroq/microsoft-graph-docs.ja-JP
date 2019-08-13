---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザーアカウント制御設定に指定できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1e26ef18691f457be74d172f9a1fc1671248ca9d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369487"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="d5d87-103">windowsUserAccountControlSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="d5d87-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="d5d87-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5d87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5d87-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5d87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5d87-106">Windows ユーザーアカウント制御設定に指定できる値。</span><span class="sxs-lookup"><span data-stu-id="d5d87-106">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="d5d87-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d5d87-107">Members</span></span>
|<span data-ttu-id="d5d87-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d5d87-108">Member</span></span>|<span data-ttu-id="d5d87-109">値</span><span class="sxs-lookup"><span data-stu-id="d5d87-109">Value</span></span>|<span data-ttu-id="d5d87-110">説明</span><span class="sxs-lookup"><span data-stu-id="d5d87-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5d87-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="d5d87-111">userDefined</span></span>|<span data-ttu-id="d5d87-112">.0</span><span class="sxs-lookup"><span data-stu-id="d5d87-112">0</span></span>|<span data-ttu-id="d5d87-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="d5d87-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="d5d87-114">常に通知</span><span class="sxs-lookup"><span data-stu-id="d5d87-114">alwaysNotify</span></span>|<span data-ttu-id="d5d87-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d5d87-115">1</span></span>|<span data-ttu-id="d5d87-116">常に通知します。</span><span class="sxs-lookup"><span data-stu-id="d5d87-116">Always notify.</span></span>|
|<span data-ttu-id="d5d87-117">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="d5d87-117">notifyOnAppChanges</span></span>|<span data-ttu-id="d5d87-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d5d87-118">2</span></span>|<span data-ttu-id="d5d87-119">アプリの変更について通知します。</span><span class="sxs-lookup"><span data-stu-id="d5d87-119">Notify on app changes.</span></span>|
|<span data-ttu-id="d5d87-120">Notifyonappのすべての非追加暗転</span><span class="sxs-lookup"><span data-stu-id="d5d87-120">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="d5d87-121">1/3</span><span class="sxs-lookup"><span data-stu-id="d5d87-121">3</span></span>|<span data-ttu-id="d5d87-122">デスクトップを暗転せずに、アプリの変更について通知します。</span><span class="sxs-lookup"><span data-stu-id="d5d87-122">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="d5d87-123">neverNotify</span><span class="sxs-lookup"><span data-stu-id="d5d87-123">neverNotify</span></span>|<span data-ttu-id="d5d87-124">2/4</span><span class="sxs-lookup"><span data-stu-id="d5d87-124">4</span></span>|<span data-ttu-id="d5d87-125">通知しません。</span><span class="sxs-lookup"><span data-stu-id="d5d87-125">Never notify.</span></span>|



