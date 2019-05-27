---
title: Privileged Identity Management
description: Azure Active Directory と Azure リソースの役割を管理する Azure AD Privileged Identity Management の API。
localization_priority: Priority
ms.openlocfilehash: 4aa4d969d97c89cf1dac3bebe8d0d6c01b68aedd
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422529"
---
# <a name="privileged-identity-management---azure-ad"></a><span data-ttu-id="6facb-103">Privileged Identity Management - Azure AD</span><span class="sxs-lookup"><span data-stu-id="6facb-103">Azure AD Privileged Identity Management</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6facb-104">[Azure Active Directory (Azure AD) Privileged Identity Management (PIM) ](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)は、お客様の組織内の重要なリソースへのアクセスを管理、制御、監視することができるサービスです。</span><span class="sxs-lookup"><span data-stu-id="6facb-104">[Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) is a service that enables you to manage, control, and monitor access to important resources in your organization.</span></span> <span data-ttu-id="6facb-105">その対象には、Azure AD や Azure リソースをはじめとする各種 Microsoft Online Services (Office 365、Microsoft Intune など) 内のリソースへのアクセスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6facb-105">This includes access to resources in Azure AD, Azure resources, and other Microsoft Online Services like Office 365 or Microsoft Intune.</span></span> <span data-ttu-id="6facb-106">Microsoft Graph には、Azure AD の役割と Azure リソースの役割を管理するために使用できる API が用意されています。</span><span class="sxs-lookup"><span data-stu-id="6facb-106">Microsoft Graph provides APIs that you can use to manage Azure AD roles and Azure resource roles.</span></span>

- [<span data-ttu-id="6facb-107">Azure AD の役割用の API</span><span class="sxs-lookup"><span data-stu-id="6facb-107">APIs for Azure AD roles</span></span>](privilegedidentitymanagement-directory.md)
- [<span data-ttu-id="6facb-108">Azure リソース の役割用の API</span><span class="sxs-lookup"><span data-stu-id="6facb-108">APIs for Azure resource roles</span></span>](privilegedidentitymanagement-resources.md)

> [!IMPORTANT]
> <span data-ttu-id="6facb-109">Azure AD の役割を管理する API は、[Azure resource API](privilegedidentitymanagement-resources.md) の名前空間と規則に従って 2019 年 6 月から 11 月の間に変更となります。</span><span class="sxs-lookup"><span data-stu-id="6facb-109">The API to manage Azure AD roles will change between June and November of 2019 to follow the namespace and convention of the [Azure resource API](privilegedidentitymanagement-resources.md).</span></span> <span data-ttu-id="6facb-110">Azure AD PIM は、Azure リソース の規則の下にあるリソースになります。</span><span class="sxs-lookup"><span data-stu-id="6facb-110">Azure AD PIM will become a resource under the Azure resource convention.</span></span> <span data-ttu-id="6facb-111">この変更がテナントに直接影響する場合は、[[Graph API を Azure AD PIM に変更するフォーム](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzfBSoy7dT5DqNLWwotW3OFUNFFMRlRLSUtRNEdDWEZHN05LT09IWjkyTS4u)] を完成させ、その他の情報やサポートを入手し、この API 変更の時刻をスケジュールできるようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6facb-111">If this change will directly affect your tenant, please complete the [Graph API change for Azure AD PIM form](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzfBSoy7dT5DqNLWwotW3OFUNFFMRlRLSUtRNEdDWEZHN05LT09IWjkyTS4u) to get additional information, support, and the ability to schedule a time for this API change.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
