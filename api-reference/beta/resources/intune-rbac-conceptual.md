---
title: Microsoft Intune での役割ベースのアクセス制御
description: テナント組織の役割ベースのアクセス制御 (RBAC) を定義して管理する Intune エンドポイント (REST) の Microsoft Graph API の一覧を示します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 24280426585014f5e397dab39daa71f8930b26c4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566389"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="9e2cc-103">Microsoft Intune での役割ベースのアクセス制御</span><span class="sxs-lookup"><span data-stu-id="9e2cc-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="9e2cc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e2cc-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e2cc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="9e2cc-107">Intune の役割ベースのアクセス制御により、だれが Intune オブジェクトに対してアクションを実行し、管理対象アプリケーション、ユーザー、デバイスを変更できるかが決まります。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="9e2cc-108">次の Graph リソースを使用して、Intune での役割ベースのアクセス制御を管理できます。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="9e2cc-109">デバイスおよびアプリ管理の割り当てられた役割の詳細</span><span class="sxs-lookup"><span data-stu-id="9e2cc-109">Device and app management assigned role details</span></span>](intune-rbac-deviceandappmanagementassignedroledetails.md)
- [<span data-ttu-id="9e2cc-110">デバイスおよびアプリ管理役割の割り当て</span><span class="sxs-lookup"><span data-stu-id="9e2cc-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="9e2cc-111">デバイスおよびアプリ管理役割の定義</span><span class="sxs-lookup"><span data-stu-id="9e2cc-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="9e2cc-112">リソース アクション</span><span class="sxs-lookup"><span data-stu-id="9e2cc-112">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="9e2cc-113">リソース操作</span><span class="sxs-lookup"><span data-stu-id="9e2cc-113">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="9e2cc-114">役割の割り当て</span><span class="sxs-lookup"><span data-stu-id="9e2cc-114">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="9e2cc-115">ロールの割り当ての範囲のタイプ</span><span class="sxs-lookup"><span data-stu-id="9e2cc-115">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="9e2cc-116">役割の定義</span><span class="sxs-lookup"><span data-stu-id="9e2cc-116">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="9e2cc-117">役割のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="9e2cc-117">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="9e2cc-118">ロールの範囲のタグ</span><span class="sxs-lookup"><span data-stu-id="9e2cc-118">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
