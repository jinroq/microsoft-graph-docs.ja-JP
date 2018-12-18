---
title: automaticUpdateMode 列挙型
description: 自動更新モードを使用可能な値です。
author: tfitzmac
ms.openlocfilehash: 01e71e51a47a06aff12dd82e132d7eb468f26229
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346992"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="5ef64-103">automaticUpdateMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="5ef64-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="5ef64-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ef64-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ef64-105">自動更新モードを使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="5ef64-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="5ef64-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="5ef64-106">Members</span></span>
|<span data-ttu-id="5ef64-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5ef64-107">Member</span></span>|<span data-ttu-id="5ef64-108">値</span><span class="sxs-lookup"><span data-stu-id="5ef64-108">Value</span></span>|<span data-ttu-id="5ef64-109">説明</span><span class="sxs-lookup"><span data-stu-id="5ef64-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ef64-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="5ef64-110">userDefined</span></span>|<span data-ttu-id="5ef64-111">0</span><span class="sxs-lookup"><span data-stu-id="5ef64-111">0</span></span>|<span data-ttu-id="5ef64-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="5ef64-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="5ef64-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="5ef64-113">notifyDownload</span></span>|<span data-ttu-id="5ef64-114">1</span><span class="sxs-lookup"><span data-stu-id="5ef64-114">1</span></span>|<span data-ttu-id="5ef64-115">ダウンロード時に通知します。</span><span class="sxs-lookup"><span data-stu-id="5ef64-115">Notify on download.</span></span>|
|<span data-ttu-id="5ef64-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="5ef64-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="5ef64-117">2</span><span class="sxs-lookup"><span data-stu-id="5ef64-117">2</span></span>|<span data-ttu-id="5ef64-118">メンテナンス時に自動インストールします。</span><span class="sxs-lookup"><span data-stu-id="5ef64-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="5ef64-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="5ef64-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="5ef64-120">3</span><span class="sxs-lookup"><span data-stu-id="5ef64-120">3</span></span>|<span data-ttu-id="5ef64-121">自動インストールおよびメンテナンス時に再起動します。</span><span class="sxs-lookup"><span data-stu-id="5ef64-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="5ef64-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="5ef64-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="5ef64-123">4</span><span class="sxs-lookup"><span data-stu-id="5ef64-123">4</span></span>|<span data-ttu-id="5ef64-124">自動インストールし、スケジュールされた時刻に再起動します。</span><span class="sxs-lookup"><span data-stu-id="5ef64-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="5ef64-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="5ef64-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="5ef64-126">5</span><span class="sxs-lookup"><span data-stu-id="5ef64-126">5</span></span>|<span data-ttu-id="5ef64-127">自動インストールし、エンドユーザーの制御に再起動します</span><span class="sxs-lookup"><span data-stu-id="5ef64-127">Auto-install and restart without end-user control</span></span>|



