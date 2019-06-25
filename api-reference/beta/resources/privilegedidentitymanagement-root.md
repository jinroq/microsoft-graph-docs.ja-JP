---
title: Privileged Identity Management
description: Azure Active Directory の役割と Azure リソースの役割を管理する Azure AD Privileged Identity Management の API。
localization_priority: Priority
ms.openlocfilehash: e8d61cb767b5471b76bc956dc5a0aeb9dc5af19f
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133811"
---
# <a name="privileged-identity-management"></a>Privileged Identity Management

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Azure Active Directory (Azure AD) Privileged Identity Management (PIM) ](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)は、お客様の組織内の重要なリソースへのアクセスを管理、制御、監視することができるサービスです。 その対象には、Azure AD や Azure リソースをはじめとする各種 Microsoft Online Services (Office 365、Microsoft Intune など) 内のリソースへのアクセスが含まれます。 Microsoft Graph には、Azure AD の役割と Azure リソースの役割を管理するために使用できる API が用意されています。

- [Azure AD の役割用の API](privilegedidentitymanagement-directory.md)
- [Azure リソース の役割用の API](privilegedidentitymanagement-resources.md)

> [!IMPORTANT]
> Azure AD の役割を管理する API は、[Azure resource API](privilegedidentitymanagement-resources.md) の名前空間と規則に従って 2019 年 6 月から 11 月の間に変更となります。 Azure AD PIM は、Azure リソース の規則の下にあるリソースになります。 この変更がテナントに直接影響する場合は、[[Graph API を Azure AD PIM に変更するフォーム](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzfBSoy7dT5DqNLWwotW3OFUNFFMRlRLSUtRNEdDWEZHN05LT09IWjkyTS4u)] を完成させ、その他の情報やサポートを入手し、この API 変更の時刻をスケジュールできるようにしてください。

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
