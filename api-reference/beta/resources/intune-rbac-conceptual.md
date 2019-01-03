---
title: Microsoft Intune での役割ベースのアクセス制御
description: 'Intune の役割ベースのアクセス制御により、だれが Intune オブジェクトに対してアクションを実行し、管理対象アプリケーション、ユーザー、デバイスを変更できるかが決まります。   '
ms.openlocfilehash: 02172a87c865a8e858725e6526f9f3959bac28c0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073892"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="73e7f-103">Microsoft Intune での役割ベースのアクセス制御</span><span class="sxs-lookup"><span data-stu-id="73e7f-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="73e7f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="73e7f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73e7f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73e7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73e7f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="73e7f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="73e7f-107">Intune の役割ベースのアクセス制御により、だれが Intune オブジェクトに対してアクションを実行し、管理対象アプリケーション、ユーザー、デバイスを変更できるかが決まります。</span><span class="sxs-lookup"><span data-stu-id="73e7f-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="73e7f-108">次の Graph リソースを使用して、Intune での役割ベースのアクセス制御を管理できます。</span><span class="sxs-lookup"><span data-stu-id="73e7f-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="73e7f-109">ロール id を割り当てられているデバイスとアプリケーションの管理</span><span class="sxs-lookup"><span data-stu-id="73e7f-109">Device and app management assigned role ids</span></span>](intune-rbac-deviceandappmanagementassignedroleids.md)
- [<span data-ttu-id="73e7f-110">デバイスおよびアプリ管理役割の割り当て</span><span class="sxs-lookup"><span data-stu-id="73e7f-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="73e7f-111">デバイスおよびアプリ管理役割の定義</span><span class="sxs-lookup"><span data-stu-id="73e7f-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="73e7f-112">リソース アクション</span><span class="sxs-lookup"><span data-stu-id="73e7f-112">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="73e7f-113">リソース操作</span><span class="sxs-lookup"><span data-stu-id="73e7f-113">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="73e7f-114">役割の割り当て</span><span class="sxs-lookup"><span data-stu-id="73e7f-114">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="73e7f-115">ロール割り当てのスコープの種類</span><span class="sxs-lookup"><span data-stu-id="73e7f-115">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="73e7f-116">役割の定義</span><span class="sxs-lookup"><span data-stu-id="73e7f-116">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="73e7f-117">役割のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="73e7f-117">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="73e7f-118">ロールのスコープのタグ</span><span class="sxs-lookup"><span data-stu-id="73e7f-118">Role scope tag</span></span>](intune-rbac-rolescopetag.md)