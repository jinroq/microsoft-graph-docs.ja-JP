---
title: Microsoft グラフ API を使用して、セキュリティ脅威の検出と保護 (プレビュー)
description: セキュリティ上の脅威の巧妙化は、世界経済に影響を与えず、エスカレートし続けます。 企業があっても認識する前に長い間、破損がよく行われます。 ビルドまたはビルドの統合、複数のソースからのセキュリティの警告を関連付けると、ユーザーの識別情報を侵害する、通知、調査、および自動化するコンテキストのデータのロックを解除しようとする脅威を検出するセキュリティ ・ ソリューションを拡張する Microsoft Graph を使用することができます。セキュリティ ・ オペレーションによって効率が向上します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 37e98203e8f031aa98b35d82110a69e434c22a3f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529930"
---
# <a name="use-the-microsoft-graph-api-for-security-threat-detection-and-protection-preview"></a><span data-ttu-id="b6b8c-105">Microsoft グラフ API を使用して、セキュリティ脅威の検出と保護 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="b6b8c-105">Use the Microsoft Graph API for security threat detection and protection (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6b8c-106">セキュリティ上の脅威の巧妙化は、世界経済に影響を与えず、エスカレートし続けます。</span><span class="sxs-lookup"><span data-stu-id="b6b8c-106">The sophistication of security threats continues to escalate, affecting the global economy.</span></span> <span data-ttu-id="b6b8c-107">企業があっても認識する前に長い間、破損がよく行われます。</span><span class="sxs-lookup"><span data-stu-id="b6b8c-107">Damage is often done long before organizations even discover it.</span></span> <span data-ttu-id="b6b8c-108">ビルドまたはビルドの統合、複数のソースからのセキュリティの警告を関連付けると、ユーザーの識別情報を侵害する、通知、調査、および自動化するコンテキストのデータのロックを解除しようとする脅威を検出するセキュリティ ・ ソリューションを拡張する Microsoft Graph を使用することができます。セキュリティ ・ オペレーションによって効率が向上します。</span><span class="sxs-lookup"><span data-stu-id="b6b8c-108">You can use Microsoft Graph to build or extend security solutions that consolidate and correlate security alerts from multiple sources, detect threats that attempt to compromise user identity, unlock contextual data to inform investigations, and automate security operations for greater efficiency.</span></span>

<span data-ttu-id="b6b8c-109">インテリジェントなセキュリティのグラフをまとめてセキュリティ ・ インテリジェンス ・から Microsoft、セキュリティ運用センター、およびパートナーからの統合型セキュリティ ・ ソリューションのエコシステムを形成するために世界中。</span><span class="sxs-lookup"><span data-stu-id="b6b8c-109">Intelligent Security Graph brings together security intelligence from within Microsoft, security operations centers, and partners from around the world to form an ecosystem of integrated security solutions.</span></span> <span data-ttu-id="b6b8c-110">機械学習、行動を監視して、クラウドのスケールを使用して、インテリジェントなセキュリティ グラフことができますより保護、検出、および迅速かつ包括的な脅威に対応します。</span><span class="sxs-lookup"><span data-stu-id="b6b8c-110">Using machine learning, behavioral monitoring, and the scale of the cloud, the Intelligent Security Graph can better protect, detect, and respond to threats quickly and comprehensively.</span></span> <span data-ttu-id="b6b8c-111">[セキュリティ API](security-api-overview.md)では、[インテリジェントなセキュリティのグラフ](https://www.microsoft.com/en-us/security/intelligence-security-api)、実践的な包括的なソリューションで支援するに接続します。</span><span class="sxs-lookup"><span data-stu-id="b6b8c-111">The [security API](security-api-overview.md) connects you to the [Intelligent Security Graph](https://www.microsoft.com/en-us/security/intelligence-security-api), empowering you with solutions that are actionable and holistic.</span></span>

<span data-ttu-id="b6b8c-112">[アイデンティティ保護リスク イベント API](identityprotection-root.md)は、[アイデンティティ保護によるリスクの検出](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started)にクエリを実行し、SIEM システムとセキュリティのアプリケーションでこれらのイベントを使用して、Azure AD プレミアム P1 と P2 のお客様に簡単にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b6b8c-112">The [identity protection risk events API](identityprotection-root.md) gives easy access for Azure AD Premium P1 and P2 customers to query [risk detections made by Identity Protection](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started) and use those events in SIEM systems and security applications.</span></span>

## <a name="see-also"></a><span data-ttu-id="b6b8c-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="b6b8c-113">See also</span></span>

- [<span data-ttu-id="b6b8c-114">セキュリティ API を使用する理由</span><span class="sxs-lookup"><span data-stu-id="b6b8c-114">Why use the security API?</span></span>](/graph/security-concept-overview#why-use-the-security-api-and-connect-with-microsoft-intelligent-security-graph)
- [<span data-ttu-id="b6b8c-115">セキュリティ API を使用して、インテリジェントなセキュリティの統合</span><span class="sxs-lookup"><span data-stu-id="b6b8c-115">Use the security API to integrate with Intelligent Security Graph</span></span>](security-api-overview.md)
- <span data-ttu-id="b6b8c-116">組織内の ID を保護するために Azure AD を使用する理由</span><span class="sxs-lookup"><span data-stu-id="b6b8c-116">[Why use Azure AD to protect identities in your organization?](/graph/security-concept-overview#why-use-azure-ad-to-protect-identities-in-your-organization)</span></span>
- [<span data-ttu-id="b6b8c-117">Azure AD Identity Protection API を使用する</span><span class="sxs-lookup"><span data-stu-id="b6b8c-117">Use the Azure AD Identity Protection API</span></span>](identityprotection-root.md)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/security-reference-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
