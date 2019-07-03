---
title: ユーザーを更新する
description: ユーザー オブジェクトのプロパティを更新します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5c4c786eedbe9dda9c4e1ed62266ea91d4adfbc5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457647"
---
# <a name="update-user"></a><span data-ttu-id="99576-103">ユーザーを更新する</span><span class="sxs-lookup"><span data-stu-id="99576-103">Update user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99576-104">[user](../resources/user.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="99576-104">Update the properties of a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="99576-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="99576-105">Permissions</span></span>
<span data-ttu-id="99576-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99576-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99576-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="99576-108">Permission type</span></span>      | <span data-ttu-id="99576-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="99576-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99576-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="99576-110">Delegated (work or school account)</span></span> | <span data-ttu-id="99576-111">ユーザーの読み取り/書き込み。すべてのユーザーとしての読み取り</span><span class="sxs-lookup"><span data-stu-id="99576-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="99576-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="99576-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99576-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99576-113">User.ReadWrite</span></span>    |
|<span data-ttu-id="99576-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="99576-114">Application</span></span> | <span data-ttu-id="99576-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99576-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="99576-116">**Passwordprofile**プロパティを更新するときには、次のアクセス許可が必要です。 directory.accessasuser.all。</span><span class="sxs-lookup"><span data-stu-id="99576-116">When updating the **passwordProfile** property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="99576-117">別のユーザーの**businessPhones**、 **mobilePhone**、またはその他の**メール**のプロパティを更新するには、管理者以外のユーザー、または次の役割のいずれかを割り当てられているディレクトリ閲覧者、ゲスト招待元、メッセージセンターリーダ、およびレポートリーダー。</span><span class="sxs-lookup"><span data-stu-id="99576-117">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="99576-118">詳細については、「 [AZURE AD で利用可能な役割](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)」の「ヘルプデスク (パスワード) 管理者」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99576-118">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="99576-119">これは、ユーザーによって付与される、またはすべての委任されたアクセス許可またはアプリケーションのアクセス許可のいずれかが付与されるアプリの場合です。</span><span class="sxs-lookup"><span data-stu-id="99576-119">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>


## <a name="http-request"></a><span data-ttu-id="99576-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="99576-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="99576-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="99576-121">Request headers</span></span>
| <span data-ttu-id="99576-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="99576-122">Header</span></span>       | <span data-ttu-id="99576-123">値</span><span class="sxs-lookup"><span data-stu-id="99576-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="99576-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="99576-124">Authorization</span></span>  | <span data-ttu-id="99576-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="99576-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="99576-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99576-127">Content-Type</span></span>  | <span data-ttu-id="99576-128">application/json</span><span class="sxs-lookup"><span data-stu-id="99576-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99576-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="99576-129">Request body</span></span>
<span data-ttu-id="99576-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="99576-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="99576-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99576-133">Property</span></span>     | <span data-ttu-id="99576-134">型</span><span class="sxs-lookup"><span data-stu-id="99576-134">Type</span></span>   |<span data-ttu-id="99576-135">説明</span><span class="sxs-lookup"><span data-stu-id="99576-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99576-136">aboutMe</span><span class="sxs-lookup"><span data-stu-id="99576-136">aboutMe</span></span>|<span data-ttu-id="99576-137">String</span><span class="sxs-lookup"><span data-stu-id="99576-137">String</span></span>|<span data-ttu-id="99576-138">ユーザーが自分自身について記述する、フリー フォームのテキスト入力フィールド。</span><span class="sxs-lookup"><span data-stu-id="99576-138">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="99576-139">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="99576-139">accountEnabled</span></span>|<span data-ttu-id="99576-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="99576-140">Boolean</span></span>| <span data-ttu-id="99576-141">アカウントが有効な場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="99576-141">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="99576-142">このプロパティは、ユーザーの作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="99576-142">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="99576-143">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="99576-143">assignedLicenses</span></span>|<span data-ttu-id="99576-144">[assignedLicense](../resources/assignedlicense.md) collection</span><span class="sxs-lookup"><span data-stu-id="99576-144">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="99576-p106">ユーザーに割り当てられているライセンス。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="99576-p106">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="99576-147">birthday</span><span class="sxs-lookup"><span data-stu-id="99576-147">birthday</span></span>|<span data-ttu-id="99576-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99576-148">DateTimeOffset</span></span>|<span data-ttu-id="99576-p107">ユーザーの誕生日。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="99576-p107">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="99576-152">businessPhones</span><span class="sxs-lookup"><span data-stu-id="99576-152">businessPhones</span></span>| <span data-ttu-id="99576-153">String コレクション</span><span class="sxs-lookup"><span data-stu-id="99576-153">String collection</span></span> | <span data-ttu-id="99576-p108">ユーザーの電話番号。注:文字列コレクションですが、このプロパティに設定できるのは 1 つの数字のみです。</span><span class="sxs-lookup"><span data-stu-id="99576-p108">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="99576-156">city</span><span class="sxs-lookup"><span data-stu-id="99576-156">city</span></span>|<span data-ttu-id="99576-157">String</span><span class="sxs-lookup"><span data-stu-id="99576-157">String</span></span>|<span data-ttu-id="99576-158">ユーザーがいる都市。</span><span class="sxs-lookup"><span data-stu-id="99576-158">The city in which the user is located.</span></span>|
|<span data-ttu-id="99576-159">country</span><span class="sxs-lookup"><span data-stu-id="99576-159">country</span></span>|<span data-ttu-id="99576-160">String</span><span class="sxs-lookup"><span data-stu-id="99576-160">String</span></span>|<span data-ttu-id="99576-161">ユーザーが配置されている国/地域。たとえば、"US" や "UK" などです。</span><span class="sxs-lookup"><span data-stu-id="99576-161">The country/region in which the user is located; for example, “US” or “UK”.</span></span>|
|<span data-ttu-id="99576-162">department</span><span class="sxs-lookup"><span data-stu-id="99576-162">department</span></span>|<span data-ttu-id="99576-163">String</span><span class="sxs-lookup"><span data-stu-id="99576-163">String</span></span>|<span data-ttu-id="99576-164">ユーザーが働いている部門の名前。</span><span class="sxs-lookup"><span data-stu-id="99576-164">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="99576-165">displayName</span><span class="sxs-lookup"><span data-stu-id="99576-165">displayName</span></span>|<span data-ttu-id="99576-166">文字列</span><span class="sxs-lookup"><span data-stu-id="99576-166">String</span></span>|<span data-ttu-id="99576-p109">アドレス帳に表示されるユーザーの名前。これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせです。このプロパティは、ユーザーの作成時に必須になります。更新時にクリアすることはできません。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="99576-p109">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="99576-171">employeeId</span><span class="sxs-lookup"><span data-stu-id="99576-171">employeeId</span></span>|<span data-ttu-id="99576-172">String</span><span class="sxs-lookup"><span data-stu-id="99576-172">String</span></span>|<span data-ttu-id="99576-173">組織によりユーザーに割り当てられた従業員 ID。</span><span class="sxs-lookup"><span data-stu-id="99576-173">The employee identifier assigned to the user by the organization.</span></span>|
|<span data-ttu-id="99576-174">givenName</span><span class="sxs-lookup"><span data-stu-id="99576-174">givenName</span></span>|<span data-ttu-id="99576-175">String</span><span class="sxs-lookup"><span data-stu-id="99576-175">String</span></span>|<span data-ttu-id="99576-176">ユーザーの名。</span><span class="sxs-lookup"><span data-stu-id="99576-176">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="99576-177">hireDate</span><span class="sxs-lookup"><span data-stu-id="99576-177">hireDate</span></span>|<span data-ttu-id="99576-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99576-178">DateTimeOffset</span></span>|<span data-ttu-id="99576-p110">ユーザーの採用日付。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="99576-p110">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="99576-182">interests</span><span class="sxs-lookup"><span data-stu-id="99576-182">interests</span></span>|<span data-ttu-id="99576-183">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="99576-183">String collection</span></span>|<span data-ttu-id="99576-184">ユーザーが自分の関心事を記述する一覧。</span><span class="sxs-lookup"><span data-stu-id="99576-184">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="99576-185">jobTitle</span><span class="sxs-lookup"><span data-stu-id="99576-185">jobTitle</span></span>|<span data-ttu-id="99576-186">String</span><span class="sxs-lookup"><span data-stu-id="99576-186">String</span></span>|<span data-ttu-id="99576-187">ユーザーの役職。</span><span class="sxs-lookup"><span data-stu-id="99576-187">The user’s job title.</span></span>|
|<span data-ttu-id="99576-188">mailNickname</span><span class="sxs-lookup"><span data-stu-id="99576-188">mailNickname</span></span>|<span data-ttu-id="99576-189">String</span><span class="sxs-lookup"><span data-stu-id="99576-189">String</span></span>|<span data-ttu-id="99576-190">ユーザーの電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="99576-190">The mail alias for the user.</span></span> <span data-ttu-id="99576-191">ユーザーの作成時に、このプロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="99576-191">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="99576-192">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="99576-192">mobilePhone</span></span>|<span data-ttu-id="99576-193">String</span><span class="sxs-lookup"><span data-stu-id="99576-193">String</span></span>|<span data-ttu-id="99576-194">ユーザーの主な携帯電話の番号。</span><span class="sxs-lookup"><span data-stu-id="99576-194">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="99576-195">mySite</span><span class="sxs-lookup"><span data-stu-id="99576-195">mySite</span></span>|<span data-ttu-id="99576-196">String</span><span class="sxs-lookup"><span data-stu-id="99576-196">String</span></span>|<span data-ttu-id="99576-197">ユーザーの個人用サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="99576-197">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="99576-198">officeLocation</span><span class="sxs-lookup"><span data-stu-id="99576-198">officeLocation</span></span>|<span data-ttu-id="99576-199">String</span><span class="sxs-lookup"><span data-stu-id="99576-199">String</span></span>|<span data-ttu-id="99576-200">ユーザーの勤務先の場所。</span><span class="sxs-lookup"><span data-stu-id="99576-200">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="99576-201">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="99576-201">onPremisesImmutableId</span></span>|<span data-ttu-id="99576-202">String</span><span class="sxs-lookup"><span data-stu-id="99576-202">String</span></span>|<span data-ttu-id="99576-203">このプロパティは、オンプレミスの Active Directory ユーザー アカウントを Azure AD ユーザー オブジェクトに関連付けるために使用します。</span><span class="sxs-lookup"><span data-stu-id="99576-203">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="99576-204">Graph で新しいユーザー アカウントを作成するとき、ユーザーの **userPrincipalName** (UPN) プロパティにフェデレーション ドメインを使用する場合は、このプロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="99576-204">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="99576-205">**重要:** **$** と **_** の文字は、このプロパティを指定するときには使用できません。</span><span class="sxs-lookup"><span data-stu-id="99576-205">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="99576-206">otherMails</span><span class="sxs-lookup"><span data-stu-id="99576-206">otherMails</span></span>|<span data-ttu-id="99576-207">String</span><span class="sxs-lookup"><span data-stu-id="99576-207">String</span></span> |<span data-ttu-id="99576-208">ユーザーの追加のメール アドレスの一覧 (例: `["bob@contoso.com", "Robert@fabrikam.com"]`)。</span><span class="sxs-lookup"><span data-stu-id="99576-208">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="99576-209">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="99576-209">passwordPolicies</span></span>|<span data-ttu-id="99576-210">String</span><span class="sxs-lookup"><span data-stu-id="99576-210">String</span></span>|<span data-ttu-id="99576-p113">ユーザーのパスワード ポリシーを指定します。この値は列挙値であり、可能な 1 つの値は "DisableStrongPassword" です。この場合は、既定のポリシーより脆弱なパスワードを指定できます。"DisablePasswordExpiration" を指定することもできます。2 つを一緒に指定することもできます。例:"DisablePasswordExpiration, DisableStrongPassword"</span><span class="sxs-lookup"><span data-stu-id="99576-p113">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="99576-215">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="99576-215">passwordProfile</span></span>|[<span data-ttu-id="99576-216">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="99576-216">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="99576-p114">ユーザーのパスワード プロファイルを指定します。プロファイルには、ユーザーのパスワードが含まれています。このプロパティは、ユーザーの作成時に必要です。プロファイルにあるパスワードは、**passwordPolicies** プロパティによって指定されている最小要件を満たす必要があります。既定では、強力なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="99576-p114">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="99576-222">pastProjects</span><span class="sxs-lookup"><span data-stu-id="99576-222">pastProjects</span></span>|<span data-ttu-id="99576-223">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="99576-223">String collection</span></span>|<span data-ttu-id="99576-224">ユーザーが過去のプロジェクトを列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="99576-224">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="99576-225">postalCode</span><span class="sxs-lookup"><span data-stu-id="99576-225">postalCode</span></span>|<span data-ttu-id="99576-226">String</span><span class="sxs-lookup"><span data-stu-id="99576-226">String</span></span>|<span data-ttu-id="99576-p115">ユーザーの住所の郵便番号。郵便番号は、ユーザーの国/地域に固有です。アメリカ合衆国では、この属性には、ZIP コードが含まれます。</span><span class="sxs-lookup"><span data-stu-id="99576-p115">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="99576-230">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="99576-230">preferredLanguage</span></span>|<span data-ttu-id="99576-231">String</span><span class="sxs-lookup"><span data-stu-id="99576-231">String</span></span>|<span data-ttu-id="99576-p116">ユーザーが設定する言語。ISO 639-1 コードに従う必要があります。たとえば "en-US" です。</span><span class="sxs-lookup"><span data-stu-id="99576-p116">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="99576-234">responsibilities</span><span class="sxs-lookup"><span data-stu-id="99576-234">responsibilities</span></span>|<span data-ttu-id="99576-235">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="99576-235">String collection</span></span>|<span data-ttu-id="99576-236">ユーザーが自分の責任の範囲を列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="99576-236">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="99576-237">schools</span><span class="sxs-lookup"><span data-stu-id="99576-237">schools</span></span>|<span data-ttu-id="99576-238">String collection</span><span class="sxs-lookup"><span data-stu-id="99576-238">String collection</span></span>|<span data-ttu-id="99576-239">ユーザーが在籍した学校を列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="99576-239">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="99576-240">skills</span><span class="sxs-lookup"><span data-stu-id="99576-240">skills</span></span>|<span data-ttu-id="99576-241">String collection</span><span class="sxs-lookup"><span data-stu-id="99576-241">String collection</span></span>|<span data-ttu-id="99576-242">ユーザーが自分のスキルを列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="99576-242">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="99576-243">state</span><span class="sxs-lookup"><span data-stu-id="99576-243">state</span></span>|<span data-ttu-id="99576-244">String</span><span class="sxs-lookup"><span data-stu-id="99576-244">String</span></span>|<span data-ttu-id="99576-245">ユーザーの住所の都道府県。</span><span class="sxs-lookup"><span data-stu-id="99576-245">The state or province in the user's address.</span></span>|
|<span data-ttu-id="99576-246">streetAddress</span><span class="sxs-lookup"><span data-stu-id="99576-246">streetAddress</span></span>|<span data-ttu-id="99576-247">String</span><span class="sxs-lookup"><span data-stu-id="99576-247">String</span></span>|<span data-ttu-id="99576-248">ユーザーの勤務先の番地。</span><span class="sxs-lookup"><span data-stu-id="99576-248">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="99576-249">surname</span><span class="sxs-lookup"><span data-stu-id="99576-249">surname</span></span>|<span data-ttu-id="99576-250">String</span><span class="sxs-lookup"><span data-stu-id="99576-250">String</span></span>|<span data-ttu-id="99576-251">ユーザーの姓。</span><span class="sxs-lookup"><span data-stu-id="99576-251">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="99576-252">usageLocation</span><span class="sxs-lookup"><span data-stu-id="99576-252">usageLocation</span></span>|<span data-ttu-id="99576-253">String</span><span class="sxs-lookup"><span data-stu-id="99576-253">String</span></span>|<span data-ttu-id="99576-254">2文字の国コード (ISO 標準 3166)。</span><span class="sxs-lookup"><span data-stu-id="99576-254">A two letter country code (ISO standard 3166).</span></span> <span data-ttu-id="99576-255">国内のサービスの利用可能性をチェックする法的な要件のためにライセンスが割り当てられるユーザーのために必要です。</span><span class="sxs-lookup"><span data-stu-id="99576-255">Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.</span></span>  <span data-ttu-id="99576-256">たとえば、"US"、"JP"、"GB" などです。</span><span class="sxs-lookup"><span data-stu-id="99576-256">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="99576-257">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="99576-257">Not nullable.</span></span>|
|<span data-ttu-id="99576-258">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="99576-258">userPrincipalName</span></span>|<span data-ttu-id="99576-259">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="99576-259">String</span></span>|<span data-ttu-id="99576-p118">ユーザーのユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 RFC 822 に基づいた、インターネット スタイルのユーザーのログイン名です。規則では、これはユーザーの電子メール名にマップされる必要があります。一般的な形式は alias@domain です。このドメインは、検証済みドメインのテナントのコレクション内に存在している必要があります。このプロパティは、ユーザーの作成時に必要です。テナントの検証済みのドメインには、[organization](../resources/organization.md) の **verifiedDomains** プロパティからアクセスできます。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="99576-p118">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="99576-267">userType</span><span class="sxs-lookup"><span data-stu-id="99576-267">userType</span></span>|<span data-ttu-id="99576-268">String</span><span class="sxs-lookup"><span data-stu-id="99576-268">String</span></span>|<span data-ttu-id="99576-269">ディレクトリ内のユーザーの種類を分類するために使用する文字列値 (“Member”、“Guest” など)。</span><span class="sxs-lookup"><span data-stu-id="99576-269">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

<span data-ttu-id="99576-270">**ユーザー**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため`PATCH` 、操作を使用して、既存の**ユーザー**インスタンスの拡張機能のカスタムプロパティで、独自のアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="99576-270">Because the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **user** instance.</span></span>

## <a name="response"></a><span data-ttu-id="99576-271">応答</span><span class="sxs-lookup"><span data-stu-id="99576-271">Response</span></span>

<span data-ttu-id="99576-272">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="99576-272">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="99576-273">例</span><span class="sxs-lookup"><span data-stu-id="99576-273">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99576-274">要求</span><span class="sxs-lookup"><span data-stu-id="99576-274">Request</span></span>
<span data-ttu-id="99576-275">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="99576-275">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="99576-276">プロトコル</span><span class="sxs-lookup"><span data-stu-id="99576-276">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="99576-277">C#</span><span class="sxs-lookup"><span data-stu-id="99576-277">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="99576-278">Javascript</span><span class="sxs-lookup"><span data-stu-id="99576-278">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="99576-279">目的-C</span><span class="sxs-lookup"><span data-stu-id="99576-279">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="99576-280">応答</span><span class="sxs-lookup"><span data-stu-id="99576-280">Response</span></span>
<span data-ttu-id="99576-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="99576-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="99576-284">関連項目</span><span class="sxs-lookup"><span data-stu-id="99576-284">See also</span></span>

- [<span data-ttu-id="99576-285">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="99576-285">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="99576-286">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="99576-286">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="99576-287">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="99576-287">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
  ]
}
-->
