---
title: ユーザーを更新する
description: ユーザー オブジェクトのプロパティを更新します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8be2b9fa3c135e710b8a0bcf819187e6cb57959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512823"
---
# <a name="update-user"></a><span data-ttu-id="c51d1-103">ユーザーを更新する</span><span class="sxs-lookup"><span data-stu-id="c51d1-103">Update user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c51d1-104">ユーザー オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c51d1-104">Update the properties of a user object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c51d1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c51d1-105">Permissions</span></span>
<span data-ttu-id="c51d1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c51d1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c51d1-108">Permission type</span></span>      | <span data-ttu-id="c51d1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c51d1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c51d1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c51d1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c51d1-111">User.ReadWrite、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c51d1-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="c51d1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c51d1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c51d1-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c51d1-113">User.ReadWrite</span></span>    |
|<span data-ttu-id="c51d1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c51d1-114">Application</span></span> | <span data-ttu-id="c51d1-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c51d1-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c51d1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c51d1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```
## <a name="request-headers"></a><span data-ttu-id="c51d1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c51d1-117">Request headers</span></span>
| <span data-ttu-id="c51d1-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c51d1-118">Header</span></span>       | <span data-ttu-id="c51d1-119">値</span><span class="sxs-lookup"><span data-stu-id="c51d1-119">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="c51d1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c51d1-120">Authorization</span></span>  | <span data-ttu-id="c51d1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c51d1-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c51d1-123">Content-Type</span></span>  | <span data-ttu-id="c51d1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c51d1-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c51d1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c51d1-125">Request body</span></span>
<span data-ttu-id="c51d1-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c51d1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c51d1-129">Property</span></span>     | <span data-ttu-id="c51d1-130">型</span><span class="sxs-lookup"><span data-stu-id="c51d1-130">Type</span></span>   |<span data-ttu-id="c51d1-131">説明</span><span class="sxs-lookup"><span data-stu-id="c51d1-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c51d1-132">aboutMe</span><span class="sxs-lookup"><span data-stu-id="c51d1-132">aboutMe</span></span>|<span data-ttu-id="c51d1-133">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-133">String</span></span>|<span data-ttu-id="c51d1-134">ユーザーが自分自身について記述する、フリー フォームのテキスト入力フィールド。</span><span class="sxs-lookup"><span data-stu-id="c51d1-134">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="c51d1-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="c51d1-135">accountEnabled</span></span>|<span data-ttu-id="c51d1-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="c51d1-136">Boolean</span></span>| <span data-ttu-id="c51d1-p104">アカウントが有効な場合は **true**。そうでない場合は **false**。このプロパティは、ユーザーの作成時に必要です。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p104">**true** if the account is enabled; otherwise, **false**. This property is required when a user is created. Supports $filter.</span></span>    |
|<span data-ttu-id="c51d1-140">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="c51d1-140">assignedLicenses</span></span>|<span data-ttu-id="c51d1-141">[assignedLicense](../resources/assignedlicense.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c51d1-141">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="c51d1-p105">ユーザーに割り当てられているライセンス。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p105">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="c51d1-144">birthday</span><span class="sxs-lookup"><span data-stu-id="c51d1-144">birthday</span></span>|<span data-ttu-id="c51d1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c51d1-145">DateTimeOffset</span></span>|<span data-ttu-id="c51d1-p106">ユーザーの誕生日。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c51d1-p106">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c51d1-149">city</span><span class="sxs-lookup"><span data-stu-id="c51d1-149">city</span></span>|<span data-ttu-id="c51d1-150">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-150">String</span></span>|<span data-ttu-id="c51d1-p107">ユーザーがいる都市。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p107">The city in which the user is located. Supports $filter.</span></span>|
|<span data-ttu-id="c51d1-153">country</span><span class="sxs-lookup"><span data-stu-id="c51d1-153">country</span></span>|<span data-ttu-id="c51d1-154">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-154">String</span></span>|<span data-ttu-id="c51d1-p108">ユーザーがいる国/地域。たとえば、「US (米国)」や「UK (英国)」です。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p108">The country/region in which the user is located; for example, “US” or “UK”. Supports $filter.</span></span>|
|<span data-ttu-id="c51d1-157">department</span><span class="sxs-lookup"><span data-stu-id="c51d1-157">department</span></span>|<span data-ttu-id="c51d1-158">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-158">String</span></span>|<span data-ttu-id="c51d1-p109">ユーザーが働いている部門の名前。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p109">The name for the department in which the user works. Supports $filter.</span></span>|
|<span data-ttu-id="c51d1-161">displayName</span><span class="sxs-lookup"><span data-stu-id="c51d1-161">displayName</span></span>|<span data-ttu-id="c51d1-162">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-162">String</span></span>|<span data-ttu-id="c51d1-p110">アドレス帳に表示されるユーザーの名前。これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせです。このプロパティは、ユーザーの作成時に必須になります。更新時にクリアすることはできません。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p110">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="c51d1-167">EmployeeID</span><span class="sxs-lookup"><span data-stu-id="c51d1-167">employeeId</span></span>|<span data-ttu-id="c51d1-168">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-168">String</span></span>|<span data-ttu-id="c51d1-169">組織がユーザーに割り当てられている従業員の識別子です。</span><span class="sxs-lookup"><span data-stu-id="c51d1-169">The employee identifier assigned to the user by the organization.</span></span> <span data-ttu-id="c51d1-170">$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-170">Supports $filter.</span></span>|
|<span data-ttu-id="c51d1-171">givenName</span><span class="sxs-lookup"><span data-stu-id="c51d1-171">givenName</span></span>|<span data-ttu-id="c51d1-172">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-172">String</span></span>|<span data-ttu-id="c51d1-p112">ユーザーの名。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p112">The given name (first name) of the user. Supports $filter.</span></span>|
|<span data-ttu-id="c51d1-175">hireDate</span><span class="sxs-lookup"><span data-stu-id="c51d1-175">hireDate</span></span>|<span data-ttu-id="c51d1-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c51d1-176">DateTimeOffset</span></span>|<span data-ttu-id="c51d1-p113">ユーザーの採用日付。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c51d1-p113">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c51d1-180">interests</span><span class="sxs-lookup"><span data-stu-id="c51d1-180">interests</span></span>|<span data-ttu-id="c51d1-181">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c51d1-181">String collection</span></span>|<span data-ttu-id="c51d1-182">ユーザーが自分の関心事を記述する一覧。</span><span class="sxs-lookup"><span data-stu-id="c51d1-182">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="c51d1-183">jobTitle</span><span class="sxs-lookup"><span data-stu-id="c51d1-183">jobTitle</span></span>|<span data-ttu-id="c51d1-184">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-184">String</span></span>|<span data-ttu-id="c51d1-p114">ユーザーの役職。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p114">The user’s job title. Supports $filter.</span></span>|
|<span data-ttu-id="c51d1-187">mailNickname</span><span class="sxs-lookup"><span data-stu-id="c51d1-187">mailNickname</span></span>|<span data-ttu-id="c51d1-188">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-188">String</span></span>|<span data-ttu-id="c51d1-p115">ユーザーの電子メール エイリアス。ユーザーの作成時に、このプロパティを指定する必要があります。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p115">The mail alias for the user. This property must be specified when a user is created. Supports $filter.</span></span>|
|<span data-ttu-id="c51d1-192">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="c51d1-192">mobilePhone</span></span>|<span data-ttu-id="c51d1-193">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-193">String</span></span>|<span data-ttu-id="c51d1-194">ユーザーの主な携帯電話の番号。</span><span class="sxs-lookup"><span data-stu-id="c51d1-194">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="c51d1-195">mySite</span><span class="sxs-lookup"><span data-stu-id="c51d1-195">mySite</span></span>|<span data-ttu-id="c51d1-196">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-196">String</span></span>|<span data-ttu-id="c51d1-197">ユーザーの個人用サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="c51d1-197">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="c51d1-198">officeLocation</span><span class="sxs-lookup"><span data-stu-id="c51d1-198">officeLocation</span></span>|<span data-ttu-id="c51d1-199">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-199">String</span></span>|<span data-ttu-id="c51d1-200">ユーザーの勤務先の場所。</span><span class="sxs-lookup"><span data-stu-id="c51d1-200">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="c51d1-201">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="c51d1-201">onPremisesImmutableId</span></span>|<span data-ttu-id="c51d1-202">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-202">String</span></span>|<span data-ttu-id="c51d1-p116">このプロパティは、オンプレミスの Active Directory ユーザー アカウントを Azure AD ユーザー オブジェクトに関連付けるために使用します。Graph で新しいユーザー アカウントを作成するとき、ユーザーの **userPrincipalName** (UPN) プロパティにフェデレーション ドメインを使用する場合は、このプロパティを指定する必要があります。**重要:\*\*\*\*$** と **_** の文字は、このプロパティを指定するときには使用できません。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p116">This property is used to associate an on-premises Active Directory user account to their Azure AD user object. This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property. **Important:** The **$** and **_** characters cannot be used when specifying this property. Supports $filter.</span></span>                            |
|<span data-ttu-id="c51d1-207">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="c51d1-207">passwordPolicies</span></span>|<span data-ttu-id="c51d1-208">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-208">String</span></span>|<span data-ttu-id="c51d1-p117">ユーザーのパスワード ポリシーを指定します。この値は列挙値であり、可能な 1 つの値は "DisableStrongPassword" です。この場合は、既定のポリシーより脆弱なパスワードを指定できます。"DisablePasswordExpiration" を指定することもできます。2 つを一緒に指定することもできます。例:"DisablePasswordExpiration, DisableStrongPassword"</span><span class="sxs-lookup"><span data-stu-id="c51d1-p117">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="c51d1-213">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="c51d1-213">passwordProfile</span></span>|[<span data-ttu-id="c51d1-214">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="c51d1-214">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="c51d1-p118">ユーザーのパスワード プロファイルを指定します。プロファイルには、ユーザーのパスワードが含まれています。このプロパティは、ユーザーの作成時に必要です。プロファイルにあるパスワードは、**passwordPolicies** プロパティによって指定されている最小要件を満たす必要があります。既定では、強力なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p118">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="c51d1-220">pastProjects</span><span class="sxs-lookup"><span data-stu-id="c51d1-220">pastProjects</span></span>|<span data-ttu-id="c51d1-221">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c51d1-221">String collection</span></span>|<span data-ttu-id="c51d1-222">ユーザーが過去のプロジェクトを列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="c51d1-222">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="c51d1-223">postalCode</span><span class="sxs-lookup"><span data-stu-id="c51d1-223">postalCode</span></span>|<span data-ttu-id="c51d1-224">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-224">String</span></span>|<span data-ttu-id="c51d1-p119">ユーザーの住所の郵便番号。郵便番号は、ユーザーの国/地域に固有です。アメリカ合衆国では、この属性には、ZIP コードが含まれます。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p119">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="c51d1-228">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="c51d1-228">preferredLanguage</span></span>|<span data-ttu-id="c51d1-229">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-229">String</span></span>|<span data-ttu-id="c51d1-p120">ユーザーが設定する言語。ISO 639-1 コードに従う必要があります。たとえば "en-US" です。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p120">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="c51d1-232">preferredName</span><span class="sxs-lookup"><span data-stu-id="c51d1-232">preferredName</span></span>|<span data-ttu-id="c51d1-233">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-233">String</span></span>|<span data-ttu-id="c51d1-234">ユーザーが設定する名前。</span><span class="sxs-lookup"><span data-stu-id="c51d1-234">The preferred name for the user.</span></span>|
|<span data-ttu-id="c51d1-235">responsibilities</span><span class="sxs-lookup"><span data-stu-id="c51d1-235">responsibilities</span></span>|<span data-ttu-id="c51d1-236">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c51d1-236">String collection</span></span>|<span data-ttu-id="c51d1-237">ユーザーが自分の責任の範囲を列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="c51d1-237">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="c51d1-238">schools</span><span class="sxs-lookup"><span data-stu-id="c51d1-238">schools</span></span>|<span data-ttu-id="c51d1-239">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c51d1-239">String collection</span></span>|<span data-ttu-id="c51d1-240">ユーザーが在籍した学校を列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="c51d1-240">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="c51d1-241">skills</span><span class="sxs-lookup"><span data-stu-id="c51d1-241">skills</span></span>|<span data-ttu-id="c51d1-242">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c51d1-242">String collection</span></span>|<span data-ttu-id="c51d1-243">ユーザーが自分のスキルを列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="c51d1-243">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="c51d1-244">state</span><span class="sxs-lookup"><span data-stu-id="c51d1-244">state</span></span>|<span data-ttu-id="c51d1-245">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-245">String</span></span>|<span data-ttu-id="c51d1-p121">ユーザーの住所の都道府県。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p121">The state or province in the user's address. Supports $filter.</span></span>|
|<span data-ttu-id="c51d1-248">streetAddress</span><span class="sxs-lookup"><span data-stu-id="c51d1-248">streetAddress</span></span>|<span data-ttu-id="c51d1-249">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-249">String</span></span>|<span data-ttu-id="c51d1-250">ユーザーの勤務先の番地。</span><span class="sxs-lookup"><span data-stu-id="c51d1-250">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="c51d1-251">surname</span><span class="sxs-lookup"><span data-stu-id="c51d1-251">surname</span></span>|<span data-ttu-id="c51d1-252">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-252">String</span></span>|<span data-ttu-id="c51d1-p122">ユーザーの姓。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p122">The user's surname (family name or last name). Supports $filter.</span></span>|
|<span data-ttu-id="c51d1-255">usageLocation</span><span class="sxs-lookup"><span data-stu-id="c51d1-255">usageLocation</span></span>|<span data-ttu-id="c51d1-256">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-256">String</span></span>|<span data-ttu-id="c51d1-p123">2 文字の国コード (ISO 規格 3166)国におけるサービスの利用可能性を確認することが法的に義務付けられているため、ライセンスを割り当てられるユーザーには必須です。例:"US"、"JP"、"GB"null 許容ではありません。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p123">A two letter country code (ISO standard 3166). Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.  Examples include: "US", "JP", and "GB". Not nullable. Supports $filter.</span></span>|
|<span data-ttu-id="c51d1-262">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c51d1-262">userPrincipalName</span></span>|<span data-ttu-id="c51d1-263">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-263">String</span></span>|<span data-ttu-id="c51d1-p124">ユーザーのユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 RFC 822 に基づいた、インターネット スタイルのユーザーのログイン名です。規則では、これはユーザーの電子メール名にマップされる必要があります。一般的な形式は alias@domain です。このドメインは、検証済みドメインのテナントのコレクション内に存在している必要があります。このプロパティは、ユーザーの作成時に必要です。テナントの検証済みのドメインには、[organization](../resources/organization.md) の **verifiedDomains** プロパティからアクセスできます。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p124">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="c51d1-271">userType</span><span class="sxs-lookup"><span data-stu-id="c51d1-271">userType</span></span>|<span data-ttu-id="c51d1-272">String</span><span class="sxs-lookup"><span data-stu-id="c51d1-272">String</span></span>|<span data-ttu-id="c51d1-p125">ディレクトリ内のユーザーの種類を分類するために使用する文字列値 (“Member”、“Guest” など)。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p125">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”. Supports $filter.</span></span>          |

<span data-ttu-id="c51d1-275">使用することが**ユーザー**のリソースは、[拡張機能](/graph/extensibility-overview)をサポートするため、`PATCH`を追加、更新、または既存の**ユーザー**インスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。</span><span class="sxs-lookup"><span data-stu-id="c51d1-275">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

## <a name="response"></a><span data-ttu-id="c51d1-276">応答</span><span class="sxs-lookup"><span data-stu-id="c51d1-276">Response</span></span>

<span data-ttu-id="c51d1-277">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c51d1-277">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="c51d1-278">例</span><span class="sxs-lookup"><span data-stu-id="c51d1-278">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c51d1-279">要求</span><span class="sxs-lookup"><span data-stu-id="c51d1-279">Request</span></span>
<span data-ttu-id="c51d1-280">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c51d1-280">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/me
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value"
}
```
##### <a name="response"></a><span data-ttu-id="c51d1-281">応答</span><span class="sxs-lookup"><span data-stu-id="c51d1-281">Response</span></span>
<span data-ttu-id="c51d1-p126">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c51d1-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="c51d1-285">関連項目</span><span class="sxs-lookup"><span data-stu-id="c51d1-285">See also</span></span>

- [<span data-ttu-id="c51d1-286">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="c51d1-286">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c51d1-287">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="c51d1-287">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- <span data-ttu-id="c51d1-288">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="c51d1-288">[Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
