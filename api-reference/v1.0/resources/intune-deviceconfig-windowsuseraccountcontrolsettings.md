---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザーアカウント制御設定に指定できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 478e525847f7f6519b3bd2cb230ce2657b409f9b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503635"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="a8250-103">windowsUserAccountControlSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="a8250-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="a8250-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8250-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8250-105">Windows ユーザーアカウント制御設定に指定できる値。</span><span class="sxs-lookup"><span data-stu-id="a8250-105">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="a8250-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="a8250-106">Members</span></span>
|<span data-ttu-id="a8250-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a8250-107">Member</span></span>|<span data-ttu-id="a8250-108">値</span><span class="sxs-lookup"><span data-stu-id="a8250-108">Value</span></span>|<span data-ttu-id="a8250-109">説明</span><span class="sxs-lookup"><span data-stu-id="a8250-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8250-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="a8250-110">userDefined</span></span>|<span data-ttu-id="a8250-111">.0</span><span class="sxs-lookup"><span data-stu-id="a8250-111">0</span></span>|<span data-ttu-id="a8250-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="a8250-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="a8250-113">常に通知</span><span class="sxs-lookup"><span data-stu-id="a8250-113">alwaysNotify</span></span>|<span data-ttu-id="a8250-114">1 </span><span class="sxs-lookup"><span data-stu-id="a8250-114">1</span></span>|<span data-ttu-id="a8250-115">常に通知します。</span><span class="sxs-lookup"><span data-stu-id="a8250-115">Always notify.</span></span>|
|<span data-ttu-id="a8250-116">notifyonappchanges</span><span class="sxs-lookup"><span data-stu-id="a8250-116">notifyOnAppChanges</span></span>|<span data-ttu-id="a8250-117">2 </span><span class="sxs-lookup"><span data-stu-id="a8250-117">2</span></span>|<span data-ttu-id="a8250-118">アプリの変更について通知します。</span><span class="sxs-lookup"><span data-stu-id="a8250-118">Notify on app changes.</span></span>|
|<span data-ttu-id="a8250-119">notifyonappのすべての非追加暗転</span><span class="sxs-lookup"><span data-stu-id="a8250-119">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="a8250-120">3 </span><span class="sxs-lookup"><span data-stu-id="a8250-120">3</span></span>|<span data-ttu-id="a8250-121">デスクトップを暗転せずに、アプリの変更について通知します。</span><span class="sxs-lookup"><span data-stu-id="a8250-121">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="a8250-122">neverNotify</span><span class="sxs-lookup"><span data-stu-id="a8250-122">neverNotify</span></span>|<span data-ttu-id="a8250-123">4 </span><span class="sxs-lookup"><span data-stu-id="a8250-123">4</span></span>|<span data-ttu-id="a8250-124">通知しません。</span><span class="sxs-lookup"><span data-stu-id="a8250-124">Never notify.</span></span>|



