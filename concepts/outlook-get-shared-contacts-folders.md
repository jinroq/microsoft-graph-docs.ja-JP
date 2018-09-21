# <a name="get-outlook-contacts-in-a-shared-folder"></a>共有フォルダーに Outlook の連絡先を取得する

顧客は Outlook を使用してお互いにフォルダーを共有し、個々の連絡先フォルダーに、「読み取り」、「作成」、「変更」または「削除」のアクセス権を提供することができます。 また、Outlook では、別のユーザーが顧客の代理として操作を行い、特定のフォルダーまたは顧客のメールボックス全体にアクセスできるように委任することも、顧客に許可しています。これは、Outlook では「委任」とも呼ばれます。

プログラムにより、Microsoft Graph では他のユーザーが共有した連絡先フォルダー内の連絡先を取得したり、共有フォルダー自体を取得することをサポートしています。 このサポートは、委任されたメールボックス内のフォルダーにも適用されます。

たとえば、Garth が John とカスタムの連絡先フォルダーを共有し、John に読み取りアクセス権を付与したとします。 ここで John がアプリにサインインし、任命を受けたアクセス許可 (Contacts.Read.Shared または Contacts.ReadWrite.Shared) を記述すれば、上記で説明したように、アプリで Garth のカスタム連絡先フォルダーとそのフォルダー内の連絡先にアクセスすることができます。

## <a name="get-a-contact-in-the-shared-folder"></a>共有フォルダー内の連絡先を取得する

Garth が John と共有したカスタムの連絡先フォルダー内の、特定の連絡先を取得することができます。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

正常に完了すれば、HTTP 200 OK と、 Garth [ の 共有連絡先フォルダーから ](../api-reference/v1.0/resources/contact.md) `{id}` によって識別された contact インスタンスが取得されます。

## <a name="get-all-contacts-in-the-shared-folder"></a>共有フォルダー内のすべての連絡先を取得する

Garth の共有連絡先フォルダー内のすべての連絡先を取得します。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

正常に完了すれば、HTTP 200 OK と、Garth の共有連絡先フォルダーの [contact](../api-reference/v1.0/resources/contact.md) インスタンスのコレクションが取得されます。

## <a name="get-the-shared-folder"></a>共有フォルダーを取得

Garth が John と共有した連絡先フォルダーを取得します。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

正常に完了すれば、HTTP 200 OK と、Garth の共有連絡先フォルダーを表す [contactFolder](../api-reference/v1.0/resources/contactfolder.md) インスタンスが取得されます。

Garth が John にメールボックス全体を委任していた場合には、同じ GET 機能が適用されます。

Garth が John と連絡先フォルダーを共有していない場合、または John にメールボックスを委任していない場合には、それらの GET 操作で Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。 


## <a name="next-steps"></a>次の手順

詳細情報:

- [Outlook 個人用連絡先を統合する理由](outlook-contacts-concept-overview.md)
- Graph v1.0 の [連絡先 API](../api-reference/v1.0/resources/contact.md) です。