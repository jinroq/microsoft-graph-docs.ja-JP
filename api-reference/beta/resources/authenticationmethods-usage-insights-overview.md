---
title: 認証方法の利用状況レポート API を使用する
description: '[認証方法] 利用状況レポートを使用すると、セルフサービスのパスワードのリセットや多要素認証 (MFA) など、エンドユーザーが Azure Active Directory の機能をどのように使用しているかを把握することができます。'
author: davidmu1
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a819276b19f2c7fdfe6ed22bd3dd07023ea08992
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645234"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a><span data-ttu-id="81bae-103">認証方法の利用状況レポート API を使用する</span><span class="sxs-lookup"><span data-stu-id="81bae-103">Working with the authentication methods usage report API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81bae-104">認証方法の利用状況レポートは、組織内のユーザーが Azure Active Directory (Azure AD) 機能を使用する方法を理解するのに役立ちます。これには、セルフサービスのパスワードの rest や多要素認証 (MFA) などがあります。</span><span class="sxs-lookup"><span data-stu-id="81bae-104">The authentication methods usage reports help you understand how users in your organization use Azure Active Directory (Azure AD) capabilities, such as self-service password rest and multi-factor authentication (MFA).</span></span>

<span data-ttu-id="81bae-105">これらのレポートは、次のような情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="81bae-105">These reports provide information such as:</span></span>

- <span data-ttu-id="81bae-106">組織にとって、どの認証方法が成功するか。</span><span class="sxs-lookup"><span data-stu-id="81bae-106">Which authentication methods are more successful for your organization.</span></span> 
- <span data-ttu-id="81bae-107">エンドユーザーが実行しているエラーの種類。</span><span class="sxs-lookup"><span data-stu-id="81bae-107">What types of errors end users are running into.</span></span>
- <span data-ttu-id="81bae-108">エンドユーザーがセルフサービスのパスワード rest と MFA の使用を採用できるようにするために実行する必要のあるキャンペーン。</span><span class="sxs-lookup"><span data-stu-id="81bae-108">What campaign you need to run to help your end users adopt the use of self-service password rest and MFA.</span></span>

## <a name="common-requests"></a><span data-ttu-id="81bae-109">一般的な要求</span><span class="sxs-lookup"><span data-stu-id="81bae-109">Common requests</span></span>

<span data-ttu-id="81bae-110">次の表に、この API で使用できる一般的な要求の一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="81bae-110">The following table lists some common requests that you can use with this API.</span></span>

| <span data-ttu-id="81bae-111">Operation</span><span class="sxs-lookup"><span data-stu-id="81bae-111">Operation</span></span> | <span data-ttu-id="81bae-112">Graph エクスプローラーで試します</span><span class="sxs-lookup"><span data-stu-id="81bae-112">Try in Graph Explorer</span></span> | <span data-ttu-id="81bae-113">説明</span><span class="sxs-lookup"><span data-stu-id="81bae-113">Description</span></span> |
| --------- | --- | ----------- |
| [<span data-ttu-id="81bae-114">getCredentialUserRegistrationcount</span><span class="sxs-lookup"><span data-stu-id="81bae-114">getCredentialUserRegistrationcount</span></span>](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta) | <span data-ttu-id="81bae-115">[/Credentialuserregistrationcount の取得](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span><span class="sxs-lookup"><span data-stu-id="81bae-115">[GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span></span> | <span data-ttu-id="81bae-116">セルフサービスのパスワードのリセットと MFA に登録されているユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="81bae-116">Get the number of users registered for self-service password reset and MFA.</span></span> |
| [<span data-ttu-id="81bae-117">getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="81bae-117">getCredentialUsageSummary</span></span>](/graph/api/resources/credentialusagesummary?view=graph-rest-beta) | [<span data-ttu-id="81bae-118">/Credentialusagesummary を取得する</span><span class="sxs-lookup"><span data-stu-id="81bae-118">GET /credentialusagesummary</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | <span data-ttu-id="81bae-119">セルフサービスのパスワードのリセットを使用してユーザーの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="81bae-119">Get the number of users using self-service password reset.</span></span> |
| [<span data-ttu-id="81bae-120">credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="81bae-120">credentialUserRegistrationDetails</span></span>](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta) | [<span data-ttu-id="81bae-121">/Credentialuserregistrationdetails の取得</span><span class="sxs-lookup"><span data-stu-id="81bae-121">GET /credentialuserregistrationdetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | <span data-ttu-id="81bae-122">セルフサービスのパスワードのリセットと MFA の登録アクティビティに関するユーザーの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="81bae-122">Get the user details for self-service password reset and MFA registration activities.</span></span> |
| [<span data-ttu-id="81bae-123">Usercredentialの詳細</span><span class="sxs-lookup"><span data-stu-id="81bae-123">userCredentialUsageDetails</span></span>](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta) | [<span data-ttu-id="81bae-124">/Usercredentialusagedetails を取得する</span><span class="sxs-lookup"><span data-stu-id="81bae-124">GET /usercredentialusagedetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | <span data-ttu-id="81bae-125">すべてのセルフサービスのパスワードリセットアクティビティのユーザー詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="81bae-125">Get user details for all self-service password reset activities.</span></span> |

## <a name="licenses"></a><span data-ttu-id="81bae-126">ライセンス</span><span class="sxs-lookup"><span data-stu-id="81bae-126">Licenses</span></span>

<span data-ttu-id="81bae-127">利用状況レポートは、セルフサービスのパスワードのリセットとテナントでの MFA を利用するライセンス機能で利用できます。</span><span class="sxs-lookup"><span data-stu-id="81bae-127">Usage reports are available for licensed features that take advantage of self-service password reset and MFA in your tenant.</span></span>

## <a name="next-steps"></a><span data-ttu-id="81bae-128">次のステップ</span><span class="sxs-lookup"><span data-stu-id="81bae-128">Next steps</span></span>

- <span data-ttu-id="81bae-129">[Azure Active Directory のセルフサービスのパスワードのリセットを展開](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-deployment)する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="81bae-129">Learn how to [deploy Azure Active Directory self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-deployment).</span></span>
- <span data-ttu-id="81bae-130">[Azure Active DIRECTORY MFA](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)を展開する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="81bae-130">Learn how to deploy [Azure Active Directory MFA](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).</span></span>
- <span data-ttu-id="81bae-131">統合された[セキュリティ情報登録](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined)を有効にする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="81bae-131">Learn how to enable [combined security info registration](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined).</span></span>



