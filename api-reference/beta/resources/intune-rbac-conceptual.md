---
title: Microsoft Intune での役割ベースのアクセス制御
description: テナント組織の役割ベースのアクセス制御 (RBAC) を定義して管理する Intune エンドポイント (REST) の Microsoft Graph API の一覧を示します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 24280426585014f5e397dab39daa71f8930b26c4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160677"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="3c4b9-103">Microsoft Intune での役割ベースのアクセス制御</span><span class="sxs-lookup"><span data-stu-id="3c4b9-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="3c4b9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3c4b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c4b9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c4b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c4b9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3c4b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="3c4b9-107">Intune の役割ベースのアクセス制御により、だれが Intune オブジェクトに対してアクションを実行し、管理対象アプリケーション、ユーザー、デバイスを変更できるかが決まります。</span><span class="sxs-lookup"><span data-stu-id="3c4b9-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="3c4b9-108">次の Graph リソースを使用して、Intune での役割ベースのアクセス制御を管理できます。</span><span class="sxs-lookup"><span data-stu-id="3c4b9-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="3c4b9-109">デバイスおよびアプリ管理の割り当てられた役割の詳細</span><span class="sxs-lookup"><span data-stu-id="3c4b9-109">Device and app management assigned role details</span></span>](intune-rbac-deviceandappmanagementassignedroledetails.md)
- [<span data-ttu-id="3c4b9-110">デバイスおよびアプリ管理役割の割り当て</span><span class="sxs-lookup"><span data-stu-id="3c4b9-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="3c4b9-111">デバイスおよびアプリ管理役割の定義</span><span class="sxs-lookup"><span data-stu-id="3c4b9-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="3c4b9-112">リソース アクション</span><span class="sxs-lookup"><span data-stu-id="3c4b9-112">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="3c4b9-113">リソース操作</span><span class="sxs-lookup"><span data-stu-id="3c4b9-113">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="3c4b9-114">役割の割り当て</span><span class="sxs-lookup"><span data-stu-id="3c4b9-114">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="3c4b9-115">ロールの割り当ての範囲のタイプ</span><span class="sxs-lookup"><span data-stu-id="3c4b9-115">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="3c4b9-116">役割の定義</span><span class="sxs-lookup"><span data-stu-id="3c4b9-116">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="3c4b9-117">役割のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="3c4b9-117">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="3c4b9-118">ロールの範囲のタグ</span><span class="sxs-lookup"><span data-stu-id="3c4b9-118">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
