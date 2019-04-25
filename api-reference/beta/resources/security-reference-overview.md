---
title: Microsoft Graph API を使用してセキュリティの脅威の検出と保護を行う (プレビュー)
description: セキュリティ上の脅威の高度化が引き続きエスカレートされ、グローバル経済に影響を与えます。 損害は、多くの場合、組織が発見する前に長く行われます。 Microsoft Graph を使用すると、複数のソースからのセキュリティの警告を統合して関連付け、ユーザー id を侵害しようとする脅威を検出し、コンテキストデータのロックを解除して調査を通知し、自動化することができます。効率性向上のためのセキュリティ操作。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 37e98203e8f031aa98b35d82110a69e434c22a3f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524464"
---
# <a name="use-the-microsoft-graph-api-for-security-threat-detection-and-protection-preview"></a><span data-ttu-id="a6c0b-105">Microsoft Graph API を使用してセキュリティの脅威の検出と保護を行う (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="a6c0b-105">Use the Microsoft Graph API for security threat detection and protection (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6c0b-106">セキュリティ上の脅威の高度化が引き続きエスカレートされ、グローバル経済に影響を与えます。</span><span class="sxs-lookup"><span data-stu-id="a6c0b-106">The sophistication of security threats continues to escalate, affecting the global economy.</span></span> <span data-ttu-id="a6c0b-107">損害は、多くの場合、組織が発見する前に長く行われます。</span><span class="sxs-lookup"><span data-stu-id="a6c0b-107">Damage is often done long before organizations even discover it.</span></span> <span data-ttu-id="a6c0b-108">Microsoft Graph を使用すると、複数のソースからのセキュリティの警告を統合して関連付け、ユーザー id を侵害しようとする脅威を検出し、コンテキストデータのロックを解除して調査を通知し、自動化することができます。効率性向上のためのセキュリティ操作。</span><span class="sxs-lookup"><span data-stu-id="a6c0b-108">You can use Microsoft Graph to build or extend security solutions that consolidate and correlate security alerts from multiple sources, detect threats that attempt to compromise user identity, unlock contextual data to inform investigations, and automate security operations for greater efficiency.</span></span>

<span data-ttu-id="a6c0b-109">インテリジェントセキュリティグラフは、Microsoft、セキュリティ運用センター、世界中のパートナーからのセキュリティインテリジェンスを一体化して、統合されたセキュリティソリューションのエコシステムを形成します。</span><span class="sxs-lookup"><span data-stu-id="a6c0b-109">Intelligent Security Graph brings together security intelligence from within Microsoft, security operations centers, and partners from around the world to form an ecosystem of integrated security solutions.</span></span> <span data-ttu-id="a6c0b-110">インテリジェントなセキュリティグラフは、機械学習、行動監視、およびクラウドの規模を使用して、脅威を迅速かつ包括的に保護、検出、応答することができます。</span><span class="sxs-lookup"><span data-stu-id="a6c0b-110">Using machine learning, behavioral monitoring, and the scale of the cloud, the Intelligent Security Graph can better protect, detect, and respond to threats quickly and comprehensively.</span></span> <span data-ttu-id="a6c0b-111">[セキュリティ API](security-api-overview.md)は、[インテリジェントセキュリティグラフ](https://www.microsoft.com/en-us/security/intelligence-security-api)に接続して、実践的で包括的なソリューションを支援します。</span><span class="sxs-lookup"><span data-stu-id="a6c0b-111">The [security API](security-api-overview.md) connects you to the [Intelligent Security Graph](https://www.microsoft.com/en-us/security/intelligence-security-api), empowering you with solutions that are actionable and holistic.</span></span>

<span data-ttu-id="a6c0b-112">[identity protection リスクイベント API](identityprotection-root.md)は、 [id 保護によってリスクの検出](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started)を照会し、SIEM システムおよびセキュリティアプリケーションでそれらのイベントを使用するための、Azure AD Premium P1 と P2 のお客様への簡単なアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="a6c0b-112">The [identity protection risk events API](identityprotection-root.md) gives easy access for Azure AD Premium P1 and P2 customers to query [risk detections made by Identity Protection](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started) and use those events in SIEM systems and security applications.</span></span>

## <a name="see-also"></a><span data-ttu-id="a6c0b-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="a6c0b-113">See also</span></span>

- [<span data-ttu-id="a6c0b-114">セキュリティ API を使用する理由</span><span class="sxs-lookup"><span data-stu-id="a6c0b-114">Why use the security API?</span></span>](/graph/security-concept-overview#why-use-the-security-api-and-connect-with-microsoft-intelligent-security-graph)
- [<span data-ttu-id="a6c0b-115">セキュリティ API を使用してインテリジェントセキュリティグラフと統合する</span><span class="sxs-lookup"><span data-stu-id="a6c0b-115">Use the security API to integrate with Intelligent Security Graph</span></span>](security-api-overview.md)
- [<span data-ttu-id="a6c0b-116">Azure AD を使用して組織内の id を保護する理由</span><span class="sxs-lookup"><span data-stu-id="a6c0b-116">Why use Azure AD to protect identities in your organization?</span></span>](/graph/security-concept-overview#why-use-azure-ad-to-protect-identities-in-your-organization)
- [<span data-ttu-id="a6c0b-117">Azure AD Identity Protection API を使用する</span><span class="sxs-lookup"><span data-stu-id="a6c0b-117">Use the Azure AD Identity Protection API</span></span>](identityprotection-root.md)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/security-reference-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
