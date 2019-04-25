---
title: groupPolicyConfigurationType 列挙型
description: グループポリシーの構成の種類
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e520bdac154ad418cd56a7984eff71ab925984d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564030"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="06fc3-103">groupPolicyConfigurationType 列挙型</span><span class="sxs-lookup"><span data-stu-id="06fc3-103">groupPolicyConfigurationType enum type</span></span>

> <span data-ttu-id="06fc3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06fc3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06fc3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="06fc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06fc3-106">グループポリシーの構成の種類</span><span class="sxs-lookup"><span data-stu-id="06fc3-106">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="06fc3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="06fc3-107">Members</span></span>
|<span data-ttu-id="06fc3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="06fc3-108">Member</span></span>|<span data-ttu-id="06fc3-109">値</span><span class="sxs-lookup"><span data-stu-id="06fc3-109">Value</span></span>|<span data-ttu-id="06fc3-110">説明</span><span class="sxs-lookup"><span data-stu-id="06fc3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06fc3-111">役割</span><span class="sxs-lookup"><span data-stu-id="06fc3-111">policy</span></span>|<span data-ttu-id="06fc3-112">.0</span><span class="sxs-lookup"><span data-stu-id="06fc3-112">0</span></span>|<span data-ttu-id="06fc3-113">ポリシーの種類は値を tattoo しません。つまり、値を削除すると、元の構成値を使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="06fc3-113">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="06fc3-114">アプリケーションが常に値を認識できるように、ポリシーの種類は、アプリケーション構成設定よりも優先されます。</span><span class="sxs-lookup"><span data-stu-id="06fc3-114">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="06fc3-115">ポリシーの種類は、ユーザーがアプリケーションのユーザーインターフェイスを使用して値を変更できないようにします。</span><span class="sxs-lookup"><span data-stu-id="06fc3-115">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="06fc3-116">優先順位</span><span class="sxs-lookup"><span data-stu-id="06fc3-116">preference</span></span>|<span data-ttu-id="06fc3-117">1 </span><span class="sxs-lookup"><span data-stu-id="06fc3-117">1</span></span>|<span data-ttu-id="06fc3-118">この設定の種類は値を tattoo するため、レジストリから値が削除されることはありません。</span><span class="sxs-lookup"><span data-stu-id="06fc3-118">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="06fc3-119">ユーザー設定の種類は、ユーザーが設定した値を上書きし、以前の値を保持しません。</span><span class="sxs-lookup"><span data-stu-id="06fc3-119">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="06fc3-120">ユーザーがアプリケーションのユーザーインターフェイスを使用して値を変更することを防止するには、ユーザー設定の種類を使用します。</span><span class="sxs-lookup"><span data-stu-id="06fc3-120">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|





